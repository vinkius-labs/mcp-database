# Unleash (Feature Toggles) MCP Server

Manage feature flags, strategies, and environments via Unleash — evaluate toggles, list projects, and monitor metrics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/unleash-feature-toggles)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect your **Unleash** instance to any AI agent and gain full control over your feature management lifecycle through natural conversation.

### What you can do

- **Feature Evaluation** — Fetch all feature flags and strategies for server-side evaluation or evaluate specific flags for client-side contexts using User IDs and properties.
- **Project & Environment Audit** — List all Unleash projects, environments, and segments to understand your infrastructure layout.
- **Flag Management** — Inspect all feature flags within specific projects to verify rollout statuses and strategy configurations.
- **Metrics & Registration** — Report SDK usage metrics and register new client or frontend instances directly through the agent.
- **User Management** — Retrieve lists of users and segments to verify targeting rules and access.

### How it works

1. Subscribe to this server
2. Enter your Unleash API URL and API Token (Admin, Client, or Frontend depending on your needs)
3. Start managing your feature rollouts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly audit environments and segments without navigating the Unleash UI
- **Product Managers** — check the status of feature toggles and rollout strategies across different projects
- **Software Engineers** — verify flag evaluations and context properties directly from the code editor


## Available Tools
- **list_environments**: Fetches all environments configured in Unleash.

List all Unleash environments
- **list_project_features**: Fetches features for a given project ID.

List all feature flags in a specific project
- **list_projects**: Fetches all projects configured in Unleash.

List all Unleash projects
- **list_segments**: Fetches all segments configured in Unleash.

List all Unleash segments
- **list_users**: Fetches all users configured in Unleash.

List all Unleash users
- **get_client_features**: Fetch all feature flags and strategies for server-side evaluation
- **report_client_metrics**: Report flag usage metrics from a backend SDK
- **register_client**: Register a new backend SDK instance
- **get_frontend_features**: Optionally provide context like userId or properties.

Fetch enabled feature flags for a specific Unleash Context
- **report_frontend_metrics**: Report flag usage metrics from a frontend SDK
- **register_frontend**: Register a new frontend SDK instance


## Installation & Usage

To install and use the **Unleash (Feature Toggles)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unleash-feature-toggles](https://vinkius.com/mcp/unleash-feature-toggles)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
