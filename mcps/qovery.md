# Qovery MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qovery)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qovery-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qovery-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Bring effortless Kubernetes and cloud deployment management to your IDE. List environments, check application states, restart pods, and deploy exact Git commits via chat.

## Description
Connect your **Qovery** infrastructure to any AI agent and bring DevOps execution directly into your coding environment.

### What you can do

- **Map your Infrastructure** — Traverse effortlessly through your Qovery Organizations, Projects, and Environments to build a complete mental map of your deployments
- **Monitor Applications** — Inspect individual microservices, check active replica counts, verify auto-deploy settings, and get real-time status updates without switching contexts to the Qovery dashboard
- **Take Action via Chat** — Trigger zero-downtime rolling restarts to cycle Kubernetes pods and refresh environment variables directly inside Claude or Cursor
- **Targeted Deployments** — Issue a fast-track deploy of a specific Git commit SHA for hotfixes or localized feature testing, all handled friction-free by the LLM

### How it works

1. Subscribe to this server
2. Supply your Qovery Organization API Token
3. Start managing your clusters and triggering deploys across your environments within seconds

### Who is this for?

- **Platform Engineers** — easily check staging environments and cluster configs while writing infrastructure-as-code paradigms
- **Full-stack Developers** — push a fix to a branch, copy the commit SHA, and just tell your agent to deploy it instantly to the dev sandbox
- **Engineering Leads** — check if the latest mission-critical app is properly scaled and healthy across multiple availability zones


## Available Tools
- **deploy_application**: Triggers an immediate deployment of a specific Git commit SHA
- **get_application**: Retrieves details for a specific Qovery application
- **get_environment**: Retrieves details for a specific Qovery environment
- **get_organization**: Retrieves details for a specific Qovery organization
- **get_project**: Retrieves details for a specific Qovery project
- **list_applications**: Lists all applications running in a specific environment
- **list_environments**: Lists all environments (Production, Staging, etc.) in a project
- **list_organizations**: Lists all Qovery organizations associated with the token
- **list_projects**: Lists all projects within a Qovery organization
- **restart_application**: Performs a zero-downtime rolling restart of a Qovery application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Qovery projects and tell me how many there are."

**🤖 AI Agent:**
> Using the `list_projects` tool on your configured organization. I retrieved 3 active projects:
1. 'E-commerce Monolith' (ID: prj-abc123x)
2. 'Payment Gateway' (ID: prj-xyz789y)
3. 'Internal Tools' (ID: prj-def456z)
Would you like to list the environments inside 'Payment Gateway'?

---

**👤 You:**
> "Check the health and limits of the application in my staging environment."

**🤖 AI Agent:**
> I checked the apps inside environment 'env-stg987'. Found 'web-frontend'.
Limits:
- CPU: 2000m
- RAM: 1024MB
- Replicas: 2 (Auto-scaling off)
It is currently showing as 'HEALTHY' and actively running.

---

**👤 You:**
> "Deploy commit 7a8f9b2 to the backend application immediately."

**🤖 AI Agent:**
> Sure, I triggered the deployment of commit SHA `7a8f9b2` for the application `backend-api` (id: app-bkn456). The deployment status is now 'DEPLOYING'. We can check back on this in a few minutes.


## Installation & Usage

To install and use the **Qovery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qovery](https://vinkius.com/mcp/qovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
