# Pulumi MCP Server

Manage cloud infrastructure via Pulumi — list stacks, track deployments, audit outputs and tag resources from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pulumi)

## Overview
**Category:** loved-by-devs
**Tools Count:** 11

## Description
Connect your **Pulumi** account to any AI agent and take full control of your infrastructure-as-code through natural conversation.

### What you can do

- **Organization Discovery** — List organizations and retrieve their details, team settings and member info
- **Stack Management** — List, create and delete stacks (infrastructure environments) across all your projects
- **Deployment Tracking** — Monitor stack update history with status (succeeded, failed, in-progress), resource changes and error logs
- **Output Inspection** — View exported output values from the latest deployment (URLs, IPs, resource IDs)
- **Tag Management** — List and set custom tags on stacks for organization and filtering (environment, team, cost-center)

### How it works

1. Subscribe to this server
2. Enter your Pulumi Access Token
3. Start managing your infrastructure from Claude, Cursor, or any MCP-compatible client

No more switching to the Pulumi Console to check deployment status or review stack outputs. Your AI acts as a dedicated infrastructure operations engineer.

### Who is this for?

- **DevOps Engineers** — quickly check stack status, review deployment history and inspect outputs without opening the Pulumi Console
- **Platform Teams** — audit infrastructure changes, track deployment success rates and manage stack tags across organizations
- **Developers** — discover available stacks, review exported endpoints and verify resource provisioning via conversation


## Available Tools
- **create_stack**: A stack is an isolated, independently configurable instance of your Pulumi program. Requires the org name, project name and stack name (e.g. "staging", "prod"). Returns the created stack with its URL.

Create a new Pulumi stack
- **delete_stack**: The stack must be empty (no resources) or force deletion must be enabled. Provide the org name, project name and stack name. WARNING: this action is irreversible.

Delete a Pulumi stack
- **get_current_user**: Returns the user's GitHub login, avatar URL, email and name. Use this to verify your access token is working correctly and to see which identity the API calls will appear as.

Get the currently authenticated Pulumi user
- **get_deployment**: Provide the org name, project name, stack name and deployment version number.

Get details for a specific Pulumi deployment
- **get_organization**: Provide the organization name (slug).

Get details for a specific Pulumi organization
- **get_stack_outputs**: Outputs are values your Pulumi program exports, such as URLs, IP addresses, resource IDs and connection strings. Useful for discovering endpoint addresses and configuration values after infrastructure deployment.

Get the exported output values from a Pulumi stack
- **get_stack**: Provide the org name, project name and stack name.

Get details for a specific Pulumi stack
- **list_deployments**: Each deployment shows its version number, status (succeeded, failed, in-progress), start/end time, resource changes (created, updated, deleted) and the user who triggered it. Use this to audit infrastructure changes and track deployment success/failure patterns.

List deployment history for a Pulumi stack
- **list_stack_tags**: Tags are key-value metadata labels used for organizing, filtering and managing stacks (e.g. environment=prod, team=platform, cost-center=engineering).

List tags on a Pulumi stack
- **list_stacks**: Each stack represents an isolated, independently configurable instance of your infrastructure (e.g. dev, staging, prod). Returns stack name, project name, last update info, resource count and whether updates are in progress.

List all stacks in a Pulumi organization
- **set_stack_tag**: Tags are used for organizing, filtering and managing stacks (e.g. key="environment", value="prod", key="team", value="platform"). Provide the org name, project name, stack name, tag name and tag value.

Set a tag on a Pulumi stack


## Installation & Usage

To install and use the **Pulumi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pulumi](https://vinkius.com/mcp/pulumi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
