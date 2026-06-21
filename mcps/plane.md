# Plane MCP Server

Manage Plane.so projects, track issues, review sprint cycles, and audit agile modules completely autonomously.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/plane)

## Overview
**Category:** productivity
**Tools Count:** 6

## Description
Equip any AI agent with direct access to your **Plane** workspace. Whether you're using Plane Cloud or self-hosting, your AI assistant can seamlessly retrieve projects, analyze agile cycles, and parse the active issues pipeline without forcing you to click through kanban boards manually.

### What you can do

- **Projects & Core Entities** — Extract isolated project architectures spanning across your Workspace, pulling high-fidelity descriptions and status parameters.
- **Agile Cycles (Sprints)** — Command the agent to list and structure your active development cycles, evaluating timelines and completion statuses.
- **Work Items (Issues)** — Perform deep sweeps over tasks and explicit tickets inside boundary states, analyzing what your engineering team is actually building.
- **Modules & Taxonomy** — Read epics (modules) and static categorization labels dictating your issue pipelines.

### How it works

1. Install this integration onto your agent layer
2. Provide your Plane Personal API Key (and optionally, your self-hosted API URL)
3. Start fetching sprints and active cycles immediately from Cursor, Claude, or any MCP client

### Who is this for?

- **Project Managers** — instantly retrieve all pending tasks in the current cycle (`list_cycles` & `list_work_items`) and summarize progress dynamically.
- **Lead Engineers** — inspect the ticket backlog without leaving your IDE; write code and verify module requirements consecutively.
- **Product Teams** — cross-reference structured modules versus labels without dealing with the visual planner interface.


## Available Tools
- **list_projects**: List projects in a Plane workspace
- **get_project**: Get specific details of a Plane project
- **list_work_items**: List work items (issues) inside a Plane project
- **list_cycles**: List cycles inside a Plane project
- **list_modules**: List modules inside a Plane project
- **list_labels**: List project labels in Plane


## Installation & Usage

To install and use the **Plane** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plane](https://vinkius.com/mcp/plane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
