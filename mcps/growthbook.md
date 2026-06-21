# GrowthBook MCP Server

Manage feature flags and experiments via GrowthBook — control environments, toggle features, and organize projects directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/growthbook)

## Overview
**Category:** developer-tools
**Tools Count:** 15

## Description
Connect your **GrowthBook** account to any AI agent to streamline your experimentation and feature management workflows through natural language.

### What you can do

- **Feature Management** — List, create, and toggle feature flags across production and staging environments to control rollouts.
- **Project Control** — Organize your experimentation roadmap by managing projects, their descriptions, and specific settings.
- **Environment Visibility** — Audit and list all configured environments to ensure flags are deployed correctly across your stack.
- **Full Lifecycle** — Create, update, or delete projects and environments as your infrastructure and team needs evolve.
- **Deep Inspection** — Retrieve detailed metadata for specific features and projects to understand their current configuration and state.

### How it works

1. Subscribe to this server
2. Enter your GrowthBook Secret Key
3. Start managing flags and experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — quickly toggle features for beta testers or check the status of an experiment without opening the dashboard
- **Engineering Teams** — manage flags and environments directly from the code editor to maintain development flow
- **DevOps Engineers** — audit environment configurations and project structures via simple natural language queries


## Available Tools
- **create_environment**: Create a new GrowthBook environment
- **create_feature**: Create a new GrowthBook feature flag (v2)
- **create_project**: Create a new GrowthBook project
- **delete_environment**: Delete a GrowthBook environment
- **delete_feature**: Delete a GrowthBook feature flag (v2)
- **delete_project**: Delete a GrowthBook project
- **get_feature**: Get a single GrowthBook feature flag (v2)
- **get_project**: Get a single GrowthBook project by ID
- **list_environments**: g., production, staging) used for per-environment feature flag control.

List all GrowthBook environments
- **list_features**: List all GrowthBook feature flags (v2)
- **list_projects**: List all GrowthBook projects
- **toggle_feature**: Toggle a GrowthBook feature flag on or off
- **update_environment**: Update an existing GrowthBook environment
- **update_feature**: Partially update a GrowthBook feature flag (v2)
- **update_project**: Edit an existing GrowthBook project


## Installation & Usage

To install and use the **GrowthBook** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growthbook](https://vinkius.com/mcp/growthbook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
