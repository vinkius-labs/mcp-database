# Northflank (Developer Cloud & Orchestration) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/northflank-developer-cloud-orchestration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage cloud infrastructure via Northflank — deploy microservices, trigger CI builds, and audit background jobs.

## Description
Connect your **Northflank** account to any AI agent and take full control of your enterprise-grade developer platform, microservice orchestration, and continuous deployment through natural conversation.

### What you can do

- **Infrastructure Orchestration** — List all managed projects and retrieve detailed regional metadata, including geographical datacenter distributions (AWS, GCP, Azure) directly from your agent
- **Service Management** — Enumerate active application instances and retrieve precise structural anatomy, including CPU throttling and RAM allocation boundaries securely
- **Live Build Injection** — Manually trigger fresh CI builds to force-refresh production assets or verify recent code merges from linked VCS (GitHub, GitLab) without opening the UI
- **Operational Control** — Gracefully cycle container replicas for specific services to recycle transient memory accumulation and restore standard execution timings natively
- **Background Job Audit** — List and inspect isolated batch and cron-jobs to monitor periodically executing processes like heavy DB aggregations or security scans
- **Security & Secret Audit** — Access metadata for logical secret groups (vaults) to verify environment variable mappings like `.env` or `DATABASE_URL` across VPC boundaries
- **Resource Provisioning** — Initialize fresh isolated project spaces or permanently tear down entire microservice ecosystems with irreversible architectural commands

### How it works

1. Subscribe to this server
2. Enter your Northflank API Token
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor microservice health and trigger production deployments through natural conversation without manual dashboard navigation
- **Backend Developers** — verify service resource allocations and audit background job statuses directly from your workspace terminal
- **Platform Teams** — manage organizational project spaces and verify secret vault mappings across multiple Northflank environments efficiently


## Available Tools
- **create_project**: Directly assigns the fundamental cloud region routing ingress requests, acting as a crucial first step in any IaC bootstrapping sequence.

Provision a brand new isolated Northflank Project space
- **delete_project**: Eliminates the Northflank project boundary entirely, severing traffic routing, killing active cron-jobs, and dropping ephemeral node.js/python backend service processes executing memory.

Permanently tear down a Project and all cascading microservices
- **get_project**: Correlates global resource restrictions backing subsequent application microservice pipelines.

Examine deeper regional metadata for a Northflank Project
- **get_service**: Useful for assessing horizontal scaling needs and verifying external domain SSL associations.

Retrieve the exact structural anatomy of a single Service
- **list_jobs**: Enumerate isolated Batch and Cron Jobs within a Project
- **list_projects**: Fetches mandatory Project IDs.

List Northflank top-level organizational Projects
- **list_secrets**: env`, `DATABASE_URL`) that subsequently map down into running services or jobs across the Northflank VPC isolation boundaries.

List Secret Group dictionaries injecting into the environments
- **list_services**: Delineates distinct Service IDs representing either Dockerized builds or native buildpack-based GitHub auto-deploy endpoints.

List explicit application/microservice instances inside a Project
- **restart_service**: Recycles transient RAM accumulation restoring standard execution timings.

Gracefully cycle container replicas for a specific Service
- **trigger_build**: Command Northflank builders to compile and deploy latest code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Northflank (Developer Cloud & Orchestration)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all services in the 'api-gateway' project"

**🤖 AI Agent:**
> I've retrieved the services for 'api-gateway' (ID: gate-123). Highlights include 'Auth-Service' (Status: Running), 'Payment-Processor' (Status: Running), and 'Notification-Node'. Would you like to check the resource allocation for the auth service?

---

**👤 You:**
> "Trigger a fresh build for service 'gate-123' in project 'proj-abc'"

**🤖 AI Agent:**
> Triggering production build… Success. I've signaled Northflank to pull the latest code from GitHub and start the build cycle for 'Auth-Service'. I'll monitor the progress and let you know once the new image is live.

---

**👤 You:**
> "Show me the secret groups configured in my project"

**🤖 AI Agent:**
> Retrieving secret vaults… I've identified 2 logical groups: 'Production-Secrets' (Group ID: sec-987) and 'Shared-API-Keys'. I can provide the names of the environment variables mapped within these groups if you'd like.


## ❓ FAQ

**Q: Can I restart my application containers through the agent without a full rebuild?**
Yes. Use the `restart_service` tool by providing your Project ID and Service ID. Your agent will signal Northflank to gracefully cycle the container replicas, effectively refreshing the running environment while maintaining your current code version.

**Q: How do I trigger a fresh build and deployment from my GitHub repository?**
The `trigger_build` tool hooks into your linked VCS. Your agent will command Northflank to fetch the latest commits from your repository and start an automated build and release cycle, promoting the new image to production immediately.

**Q: Can my agent check the status of my periodic cron-jobs?**
Absolutely. Use the `list_jobs` tool to identify all isolated background processes within a project. Your agent will report the current execution statuses and schedule parameters for both ad-hoc batch tasks and recurring cron-jobs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/northflank-developer-cloud-orchestration](https://vinkius.com/mcp/northflank-developer-cloud-orchestration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Northflank (Developer Cloud & Orchestration)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `northflank-developer-cloud-orchestration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Northflank (Developer Cloud & Orchestration)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "northflank-developer-cloud-orchestration": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
