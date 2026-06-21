# data.world MCP Server

Equip your AI agent to discover and manage data assets, projects, and queries directly via the data.world API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dataworld)

## Overview
**Category:** knowledge-management
**Tools Count:** 10

## Description
Integrate **data.world**, the enterprise data catalog and collaborative data platform, directly into your AI workflow. Discover datasets, monitor data projects, and explore saved queries and insights using natural language.

### What you can do

- **Data Discovery** — Search the entire data.world catalog for relevant datasets and projects.
- **Asset Management** — List and retrieve detailed information for datasets and projects you own or manage.
- **Collection Oversight** — Explore curated collections of data assets within your organization.
- **Query & Insight Access** — List saved SQL/SPARQL queries and published insights for your data projects.

### How it works

1. Connect the data.world integration to your AI assistant.
2. Authorize using your data.world API Token (found in your user settings).
3. Manage your data catalog and collaborative projects through intuitive conversation.

### Who is this for?

- **Data Scientists & Analysts** — Quickly find datasets and retrieve query definitions for research.
- **Data Stewards** — Monitor project status and audit data assets via chat.
- **Knowledge Managers** — Explore organizational collections and insights during data planning.


## Available Tools
- **get_dataset_details**: Includes field definitions, file listings, tags, and license information.

Get detailed information for a specific dataset
- **get_my_profile**: world. Returns profile attributes including username, display name, and account-level permissions.

Retrieve metadata for the current authenticated user
- **get_project_details**: Resolves project members, associated objective, and the current status of linked resources.

Get detailed information for a specific project
- **list_recent_activity**: Returns a stream of activity logs including dataset updates, project contributions, and new collection entries.

List recent activities in your data.world account
- **list_my_collections**: Returns collection identifiers, descriptions, and item counts.

List all collections you own or manage
- **list_dataset_queries**: Returns a list of saved query definitions, including their language (SQL/SPARQL) and creator metadata.

List all saved SQL or SPARQL queries for a dataset
- **list_my_datasets**: world catalog for datasets owned by the authenticated user. Returns a list of dataset metadata including title, visibility (public/private), and timestamp of last modification.

List all datasets you own on data.world
- **list_project_insights**: Insights represent documented findings and data visualizations attached to the project workspace.

List all insights published within a project
- **list_my_projects**: Returns project summaries including role (owner/contributor), creation date, and linked datasets.

List all projects you own on data.world
- **search_catalog**: world index. Supports full-text search across titles, descriptions, and tags. Returns a ranked list of matching resources.

Search for datasets and projects across data.world


## Installation & Usage

To install and use the **data.world** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dataworld](https://vinkius.com/mcp/dataworld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
