# airfocus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airfocus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airfocus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airfocus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Prioritize your product roadmap, score features by impact, and align your team on what to build next with strategic clarity.

## Description
Connect your **airfocus** account to any AI agent and take full control of your product management and strategic roadmapping workflows through natural conversation.

### What you can do

- **Workspace & Roadmap Orchestration** — List all strategic workspaces programmatically, retrieving detailed metadata and custom fields tailored for every product board
- **Item Lifecycle Management** — Programmatically create and update tasks, features, and initiatives, monitoring status transitions and high-fidelity descriptions in real-time
- **Prioritization Intelligence** — Retrieve and update prioritization scores and custom field data to coordinate your product strategy and team alignment perfectly
- **Cross-functional Sync** — Ensure your engineering context matches product roadmaps by querying specific item details directly through your agent
- **Infrastructure Monitoring** — Access high-fidelity metadata for your workspaces and manage field definitions to maintain a perfectly coordinated project environment

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your airfocus Member settings
3. Start orchestrating your product strategy from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to check feature statuses or roadmap priorities. Your AI acts as your dedicated product manager and strategic coordinator.

### Who is this for?

- **Product Managers** — instantly retrieve roadmap summaries and update prioritization scores using natural language commands
- **Engineering Teams** — check product requirements and sync metadata without leaving your creative workspace
- **Strategic Leads** — automate the oversight of roadmap metrics and workspace distribution through simple AI queries


## Available Tools
- **create_airfocus_item**: Create an item
- **get_airfocus_item**: Get item details
- **list_airfocus_fields**: List custom fields
- **list_airfocus_items**: List workspace items
- **list_airfocus_workspaces**: List all workspaces
- **update_airfocus_item**: Update an item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **airfocus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all items in the 'Product Roadmap' workspace (ID: '123')."

**🤖 AI Agent:**
> I've retrieved your roadmap items. You currently have 15 active features, including 'AI Search' (Status: In Progress) and 'Mobile App v2'. Would you like the detailed high-fidelity metadata for any of these?

---

**👤 You:**
> "Create a new feature 'User Analytics' in workspace '123'."

**🤖 AI Agent:**
> Item created! I've successfully registered 'User Analytics' in specified workspace (ID: 123). It's now visible on your priority board. Shall I list the custom fields for this board to set a priority score?

---

**👤 You:**
> "Show the custom fields for workspace '123'."

**🤖 AI Agent:**
> Accessing board configuration... Workspace 123 has 5 custom fields including 'Impact', 'Effort', and 'Strategic Fit'. I've retrieved the high-fidelity IDs for these fields to help with automated scoring. Need a summary of the values?


## Installation & Usage

To install and use the **airfocus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airfocus](https://vinkius.com/mcp/airfocus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
