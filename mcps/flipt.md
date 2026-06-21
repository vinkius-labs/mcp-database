# Flipt MCP Server

Manage feature flags and rollouts via Flipt — list namespaces, flags, segments, and rules directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flipt)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Flipt** instance to any AI agent to orchestrate feature management and progressive delivery through natural conversation.

### What you can do

- **Flag Management** — List and inspect feature flags across different namespaces to understand your current feature states
- **Targeting & Segments** — Retrieve segments and create constraints to define specific user subsets for targeted rollouts
- **Rollout Control** — List rules and rollouts, and create distributions to manage percentage-based releases and canary deployments
- **Variants** — Create and manage flag variants to return different values based on evaluation logic
- **Auth & Infrastructure** — List authentication tokens and namespaces to understand your environment's structure and access levels

### How it works

1. Subscribe to this server
2. Enter your Flipt URL and API Token
3. Start managing your feature flags from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly audit rollout configurations and namespace partitions without leaving the terminal or IDE
- **Product Managers** — check the status of feature flags and segments to verify release progress
- **Developers** — create variants and constraints directly while coding to speed up feature implementation


## Available Tools
- **create_constraint**: Create a constraint for a segment
- **create_distribution**: Create a distribution for a rule
- **create_variant**: Create a new variant for a flag
- **list_flags**: List flags in a namespace
- **list_namespaces**: List all namespaces
- **list_rollouts**: List rollouts for a flag
- **list_rules**: List rules for a flag
- **list_segments**: List segments in a namespace
- **list_tokens**: List authentication tokens


## Installation & Usage

To install and use the **Flipt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flipt](https://vinkius.com/mcp/flipt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
