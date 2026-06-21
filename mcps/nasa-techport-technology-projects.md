# NASA TechPort (Technology Projects) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-techport-technology-projects)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-techport-technology-projects-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-techport-technology-projects-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore NASA's technology project portfolio—search projects, track funding opportunities, and analyze R&D taxonomies directly.

## Description
Connect to **NASA TechPort** to explore the agency's comprehensive resource for technology project data. This MCP server allows AI agents to navigate thousands of active and completed NASA research initiatives, providing deep insights into the future of aerospace and space exploration.

### What you can do

- **Project Discovery** — List and fetch detailed metadata, descriptions, and status updates for specific NASA technology projects using `list_projects` and `get_project`.
- **Funding & Opportunities** — Search for open funding opportunities, check maximum funding amounts, and export data for analysis using `search_opportunities` and `export_opportunities`.
- **Organizational Insights** — Identify participating organizations, their types, and roles in various programs via `list_organizations` and `search_organizations`.
- **Taxonomy Navigation** — Explore the NASA technology roadmap through structured taxonomy trees and nodes using `get_taxonomy_tree`.
- **Program Analysis** — Retrieve detailed information about NASA programs and their associated technology portfolios with `list_programs`.

### How it works

1. Subscribe to this server
2. Enter your NASA API Key (obtained from api.nasa.gov)
3. Start querying NASA's R&D database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — quickly find existing NASA research to avoid duplication and find collaboration points.
- **Aerospace Engineers** — stay updated on the latest technological advancements in propulsion, materials, and life support.
- **Policy Makers & Analysts** — track NASA's technology investments and program distributions across different organizations.


## Available Tools
- **search_object_all_data**: Conduct a search for all objects with all fields included
- **list_organization_types**: List available organization types
- **list_organizations**: List organizations matching filters
- **list_programs**: List all programs
- **list_projects**: Requires updatedSince query parameter.

List available technology project IDs
- **list_taxonomies**: List taxonomy roots
- **export_opportunities**: Export funding opportunities
- **get_api_spec**: Get the Swagger/OpenAPI specification for the API
- **get_enum**: Get enumerations for a specific field name
- **get_max_funding_amount**: Get the maximum funding amount available
- **get_nonce**: Refresh the user nonce for secure sessions
- **get_opportunity**: Get data for a specific opportunity
- **get_organization**: Get detailed information for a specific organization
- **get_program**: Get detailed information for a specific program
- **get_project**: Get detailed information about a specific technology project
- **get_schema**: Get the object schema for a specific type
- **get_taxonomy**: Get a taxonomy root and its children
- **get_taxonomy_tree**: Get a full taxonomy in a tree format
- **list_contacts**: List contacts in TechPort
- **list_enums**: List enumerations for various fields used in the API
- **list_opportunities**: List all funding opportunities
- **list_taxonomy_nodes**: List taxonomy nodes filtered by root ID, level, or code
- **predict_drex**: Retrieve Destination Area recommendations for a project description
- **predict_trex**: Retrieve taxonomy recommendations for a technology description
- **search_object_advanced**: Search on an object type based on complex criteria
- **search_object**: Search on a given object type using a query string
- **search_opportunities**: Search funding opportunities based on passed criteria
- **search_organizations**: Search organizations based on provided criteria
- **submit_feedback**: Submit user feedback to the TechPort team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA TechPort (Technology Projects)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all NASA technology projects that have been updated since 2024-01-01."

**🤖 AI Agent:**
> I've found several projects updated since then. Here are the IDs: 14523, 14688, and 14701. Would you like me to fetch the details for any of these specific projects?

---

**👤 You:**
> "Show me the full details for NASA project ID 94566."

**🤖 AI Agent:**
> Project 94566 is titled 'Advanced Propulsion Concepts'. It is currently in the 'Active' stage and is led by the Marshall Space Flight Center. The primary goal is to develop high-efficiency thrusters for deep space missions.

---

**👤 You:**
> "Search for funding opportunities related to 'autonomous robotics'."

**🤖 AI Agent:**
> I found 2 opportunities matching 'autonomous robotics'. One is a Small Business Innovation Research (SBIR) call with a max funding of $150,000. Would you like the full criteria?


## Installation & Usage

To install and use the **NASA TechPort (Technology Projects)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-techport-technology-projects](https://vinkius.com/mcp/nasa-techport-technology-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
