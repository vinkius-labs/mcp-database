# Railway MCP Server

Manage cloud deployments via Railway — list projects, inspect services, track deployments and manage variables and volumes from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/railway-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 11

## Description
Connect your **Railway** account to any AI agent and take full control of your cloud deployments through natural conversation.

### What you can do

- **Project Discovery** — List all projects and retrieve their details including names, descriptions and timestamps
- **Environment Management** — View all deployment environments (production, staging, development) per project
- **Service Inspection** — List all services (containers, databases, plugins) within a project, optionally filtered by environment
- **Deployment Tracking** — View deployment history with status (success, failed, deploying) for any service
- **Variable Management** — List, set and delete environment variables for services in specific environments
- **Volume Audit** — List persistent storage volumes with their sizes and associated services
- **Domain Management** — Review custom domains and their SSL certificate status for any service

### How it works

1. Subscribe to this server
2. Enter your Railway Personal Access Token
3. Start managing your cloud deployments from Claude, Cursor, or any MCP-compatible client

Stop clicking through the Railway dashboard to check deployment status or manage environment variables. Your AI acts as a dedicated cloud operations engineer.

### Who is this for?

- **Developers** — inspect services, track deployments and manage environment variables without leaving your IDE
- **DevOps Engineers** — audit project configurations, review deployment statuses and manage persistent volumes
- **Team Leads** — monitor project health, environment segregation and variable security across services


## Available Tools
- **delete_variable**: Provide the service_id, environment_id and variable name. WARNING: the variable will no longer be available to deployments after deletion.

Delete an environment variable from a Railway service
- **list_deployments**: Each deployment has an ID, status (success, failed, deploying, removed), creation and update timestamps. Use the service_id from list_services.

List deployments for a Railway service
- **list_domains**: Each domain has an ID, the domain string and SSL status (verified, pending, failed). Use this to audit which services are accessible via custom URLs.

List custom domains for a Railway service
- **list_environments**: g. production, staging, development) configured within a specific Railway project. Each environment has its own set of services, variables and deployments. Use the project_id from list_projects.

List environments in a Railway project
- **get_project**: Provide the project ID obtained from list_projects.

Get details for a specific Railway project
- **list_projects**: Each project groups related services, environments and deployments together. Returns project ID, name, description and timestamps. Use this as the starting point for all Railway operations.

List all Railway projects
- **list_services**: Optionally filter by environment_id to see services in a specific environment only. Each service represents a deployable unit like a web app, API, database or Redis instance.

List services in a Railway project
- **set_variable**: Requires the service_id, environment_id, variable name and value. The variable will be available to all deployments of that service in the given environment.

Set an environment variable for a Railway service
- **list_variables**: Each variable has a name and scope (service, environment, project). Variable values are NOT returned for security — only names and scopes. Use service_id and environment_id from their respective list tools.

List environment variables for a Railway service
- **get_viewer**: Use this to verify which account the API token belongs to.

Get current authenticated Railway user details
- **list_volumes**: Each volume has an ID, name, associated service ID and size in gigabytes. Volumes provide persistent storage that survives deployments and restarts.

List persistent volumes in a Railway project


## Installation & Usage

To install and use the **Railway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/railway-alternative](https://vinkius.com/mcp/railway-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
