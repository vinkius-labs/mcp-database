# Insomnia (Collaborative API Design) MCP Server

Manage API designs and collections via Insomnia — list organizations, projects, and files, and audit API specs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/insomnia-collaborative-api-design)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **Insomnia Cloud** account to any AI agent and take full control of your collaborative API development and design lifecycle through natural conversation.

### What you can do

- **Organization & Project Management** — List all organizations and team projects to navigate your API design and debugging environments effortlessly
- **API File Inspection** — Retrieve exact content payloads for design documents and request collections, including full OpenAPI/Swagger specifications
- **Environment Audit** — List project environments and variable counts to understand stage-specific configurations like base URLs and auth tokens
- **Team Collaboration** — Identify registered members and roles in your organization and track collaborative progress across parallel feature branches
- **Mock Server Monitoring** — Analyze deployed mock servers linked to your projects, including their operational states and hosted endpoints
- **AI Insights** — Query AI-powered request logs and test suggestions generated within your Insomnia organization to improve API quality

### How it works

1. Subscribe to this server
2. Enter your Insomnia Personal Access Token
3. Start managing your API lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **API Developers** — fetch OpenAPI specs and request collections directly through natural conversation without opening the desktop app
- **QA Engineers** — audit mock server statuses and environment configurations to ensure accurate test execution
- **Software Architects** — monitor API design progress across multiple team projects and feature branches efficiently


## Available Tools
- **list_orgs**: Use this to find the appropriate org_id needed for subsequent project or file operations.

List all organizations on Insomnia Cloud. Insomnia (by Kong) is a leading API design, debugging, and testing tool supporting REST, GraphQL, gRPC, and WebSockets. Returns org names, IDs, and member counts
- **list_projects**: Projects contain design files, requests, environments, and mock servers.

List team projects in an Insomnia organization. Projects group API specs, collections, and environments. Returns project names and IDs
- **list_files**: Use to locate the specific file_id for fetching API definitions.

List files in an Insomnia project. Files include API specs (OpenAPI/Swagger), request collections, and design documents. Returns names, types, and last modified dates
- **get_file**: Get full details of an Insomnia file including name, type, content (spec/collection JSON), and version history
- **list_branches**: Useful to track collaborative progress across multiple parallel feature branches.

List branches of an Insomnia file. Git-like branching for API specs and collections. Returns branch names and statuses
- **list_collaborators**: List members in an Insomnia organization. Returns usernames, emails, roles, and access levels
- **list_ai_requests**: Exposes usage metrics and metadata surrounding Insomnia AI interactions.

List AI-powered API requests generated in an Insomnia organization. Returns AI-generated specs and test suggestions
- **get_user**: Helps audit basic permission identity context.

Get the authenticated Insomnia user profile. Returns username, email, plan, and org memberships
- **list_environments**: Environments are the primary way Insomnia abstracts configuration, injecting values into execution payloads.

List environments in an Insomnia project. Environments hold variables (base URLs, tokens) for different stages. Returns env names and variable counts
- **list_mocks**: List mock servers in an Insomnia project. Mock servers simulate API responses for testing. Returns mock names, URLs, and statuses


## Installation & Usage

To install and use the **Insomnia (Collaborative API Design)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/insomnia-collaborative-api-design](https://vinkius.com/mcp/insomnia-collaborative-api-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
