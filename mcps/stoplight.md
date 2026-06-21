# Stoplight MCP Server

Connect your AI to Stoplight. Design, document, and manage your API lifecycle, exploring workspaces and schemas effortlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stoplight)

## Overview
**Category:** developer-tools
**Tools Count:** 7

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


## Installation & Usage

To install and use the **Stoplight** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stoplight](https://vinkius.com/mcp/stoplight)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
