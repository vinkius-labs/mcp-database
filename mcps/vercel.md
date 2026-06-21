# Vercel MCP Server

Bring your Vercel deployment infrastructure into chat. Control project domains, trigger manual builds, and inspect deployment status natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vercel)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Embed your **Vercel** continuous integration ecosystem into the mind of your AI agent. Perform advanced DevOps commands via chat, bypassing the Vercel web UI and checking application states natively within your IDE.

### What you can do

- **Project Control** — Command your assistant to list your current architecture portfolio, examine Git environment settings, or spin up new Vercel boundary projects dynamically from the chat window.
- **Deployment Management** — Trace live builds. Request the active CI/CD execution status on recent commits, fetch preview URLs upon build completion, or ruthlessly cancel stalled serverless compilations.
- **Manual Deploy Triggers** — Skip the Github pushes. You can explicitly command a forced build on specific repository tags directly through the MCP integration when hot-fixing.
- **Domain Auditing** — Ask the agent to map out the DNS and SSL status of your custom root domains, parsing current subdomain routing alias tables clearly.

### How it works

1. Subscribe your workspace to this connector
2. Introduce your personal Vercel API Token for authorization
3. Engage Claude or Cursor to manage deployment lifecycles seamlessly

### Who is this for?

- **Frontend Engineers** — trigger new manual Next.js deployments inside Cursor directly after fixing a tricky CSS bug, tracking the CI steps silently while coding the next feature.
- **DevOps Architects** — perform rapid audits of linked domain structures and DNS alias health checks across the organization's array using basic conversational inputs.
- **Quality Assurance** — instantly pull the most recent Preview URL generated from the target branch staging deployments without hunting for the Vercel notification link.


## Available Tools
- **cancel_active_build**: Aborts an ongoing Vercel compilation pipeline
- **trigger_github_deployment**: Provide the project name and Git ref.

Triggers a new Vercel build from a specific GitHub reference
- **create_project**: Provide a name and framework slug.

Creates a new Vercel project
- **list_account_domains**: Lists high-level apex domains managed by Vercel
- **list_projects**: Lists all Vercel projects in the account
- **delete_project**: This action is irreversible.

Permanently removes a Vercel project
- **get_deployment_details**: Retrieves details for a specific deployment execution
- **get_project_details**: Retrieves detailed configuration for a specific project
- **list_project_aliases**: Lists specific subdomain routing mappings for a project
- **list_deployments**: Lists recent CI/CD builds for a specific project


## Installation & Usage

To install and use the **Vercel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vercel](https://vinkius.com/mcp/vercel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
