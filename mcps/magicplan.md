# Magicplan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magicplan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/magicplan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/magicplan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage floor plans, spatial data, and financial estimates via the Magicplan REST API.

## Description
Connect your **Magicplan** workspace to any AI agent to automate your architectural and estimation workflows. This MCP server enables your agent to interact with floor plans, retrieve precise spatial measurements, and access detailed financial estimates directly from natural language interfaces.

### What you can do

- **Project Oversight** — List all architectural projects and retrieve detailed metadata and status updates
- **Spatial Intelligence** — Access full floor plan spatial data including floors, rooms, and individual object placements
- **Precise Measurements** — Retrieve numeric statistics such as area, perimeter, and volume for any plan or specific room
- **Estimation Audit** — Access comprehensive financial breakdowns including labor, materials, taxes, and itemized positions
- **User Management** — List collaborators and manage workspace access across your architectural teams
- **Data Collection** — Query inspection forms and survey data attached directly to your floor plans

### How it works

1. Subscribe to this server
2. Enter your Magicplan Customer ID and API Key
3. Start managing your architectural data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Architects & Surveyors** — Quickly query floor plan measurements and project statuses via natural language commands
- **Construction Managers** — Monitor project estimates and financial breakdowns without leaving your dev tools
- **Real Estate Professionals** — Automate the extraction of spatial metadata and floor plan statistics effortlessly


## Available Tools
- **list_project_estimates**: List all financial estimates for a project
- **list_available_forms**: List all data collection forms (checklists)
- **get_estimate_details**: Get full financial breakdown for an estimate
- **get_project_floor_plan**: Get full spatial data for a project
- **get_project_details**: Get metadata for a specific project
- **get_plan_form_data**: Retrieve forms attached to a specific plan
- **get_plan_measurements**: Get numeric measurements for a plan
- **list_magicplan_projects**: List all floor plan projects
- **list_workspace_users**: List all users in the Magicplan workspace
- **get_workspace_info**: Get configuration for the current workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magicplan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all architectural projects in my Magicplan workspace."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Beach House Renovation (ID: 123)', 'Downtown Office (ID: 456)', and 'Modern Loft (ID: 789)'.

---

**👤 You:**
> "Show the floor plan measurements for project ID '123'."

**🤖 AI Agent:**
> I've retrieved the measurements. For Project 123, the total area is 120.5 sqm, with a perimeter of 45.2 m. The Master Bedroom (Room ID: abc) has an area of 18.2 sqm.

---

**👤 You:**
> "Get the financial breakdown for estimate 'est-987' in project '456'."

**🤖 AI Agent:**
> I've fetched the breakdown for estimate est-987. The total is $5,450.00, including $2,100.00 for labor and $3,350.00 for materials. There are 12 individual line items listed.


## Installation & Usage

To install and use the **Magicplan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magicplan](https://vinkius.com/mcp/magicplan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
