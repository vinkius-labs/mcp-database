# Stoplight MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stoplight)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stoplight-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stoplight-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to Stoplight. Design, document, and manage your API lifecycle, exploring workspaces and schemas effortlessly.

## Description
Integrate the industry-leading API design and documentation capabilities of **Stoplight** into your conversational AI workflows. Empower your engineering teams to explore workspaces, evaluate OpenAPI schemas, and audit API projects natively from their conversational assistant. Securely map your AI to your Stoplight workspace, enabling the orchestration of complex documentation tasks, project navigation, and architectural reviews naturally without switching contexts or opening complex dashboards.

### What you can do

- **Workspace Exploration** — Rapidly inspect top-level organizational containers invoking `list_workspaces`, and track operational changes programmatically leveraging `list_workspace_activity`.
- **Project Management** — Audit your API documentation repositories cataloging initiatives securely using `list_projects`, and retrieve full visibility metadata invoking `get_project_details`.
- **Schema & Documentation Discovery** — Dive deeply into specific documentation structures retrieving files, endpoints, and models leveraging `list_project_nodes`, and parse their raw text safely utilizing `get_node_details`.
- **Team & Governance** — Map project ownership accurately and enforce governance metrics iteratively assigning roles retrieving authorized contributors naturally via `list_workspace_members`.

### How it works

1. Install the Stoplight MCP module securely authenticating it to your organizational AI interface.
2. In the MCP configurations, provide your `STOPLIGHT_WORKSPACE` slug and a valid `STOPLIGHT_TOKEN` generated directly from your Stoplight workspace settings.
3. Prompt the AI: "List the latest active endpoints from our 'core-billing-api' project and retrieve the detailed schema documentation for the processing node."

### Who is this for?

- **API Architects** — Accelerate API design reviews by instantly accessing endpoints and OpenAPI models naturally via your terminal without leaving your coding environment.
- **Technical Writers** — Discover and organize large scale API documentation landscapes rapidly summarizing updates directly from recent workspace activity logs.
- **Backend Engineers** — Resolve integration dependencies efficiently by querying endpoint models across independent Stoplight projects precisely and securely.


## Available Tools
- **get_node_details**: Retrieves details for a specific documentation node
- **get_project_details**: Retrieves details for a specific Stoplight project
- **list_workspace_activity**: Lists recent activity logs for a Stoplight workspace
- **list_workspace_members**: Lists all members of a Stoplight workspace
- **list_project_nodes**: Lists all documentation nodes (files, endpoints, models) within a project
- **list_projects**: Lists all projects in a specific Stoplight workspace
- **list_workspaces**: Lists all accessible Stoplight workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stoplight** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Stoplight projects and show recent workspace activity."

**🤖 AI Agent:**
> Connected successfully.
**Projects (`list_projects`)**:
- `Payment V2 Refactor`
- `Internal Logistics API`

**Recent Activity (`list_workspace_activity`)**:
- *alex.dev* updated the `POST /transactions` endpoint with new security parameters.

---

**👤 You:**
> "Retrieve the detailed schema documentation for the processing node in our core billing API project."

**🤖 AI Agent:**
> Accessing workspace files...

**Node Details (`get_node_details`)**:
Extracted the OpenAPI schema for the `processing` endpoint. It expects a payload including `transactionId`, `amount`, and `currency`. Validation is active. How would you like to review these definitions?

---

**👤 You:**
> "List all active members in the current workspace."

**🤖 AI Agent:**
> Checking organizational permissions...

**Workspace Members (`list_workspace_members`)**:
- Jane Doe (Admin)
- John Smith (Editor)
- Alex Dev (Viewer)

All 3 members are currently active and mapped to active API projects.


## Installation & Usage

To install and use the **Stoplight** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stoplight](https://vinkius.com/mcp/stoplight)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
