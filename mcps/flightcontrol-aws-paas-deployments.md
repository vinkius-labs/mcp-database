# Flightcontrol (AWS PaaS Deployments) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flightcontrol-aws-paas-deployments)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deploy and manage AWS infrastructure via Flightcontrol — list projects, manage environments, and scale services directly from any AI agent.

## Description
Connect your **Flightcontrol** account to any AI agent to orchestrate your AWS deployments and infrastructure through natural conversation.

### What you can do

- **Project Management** — List all projects and automate the creation of new ones with Git repository integration.
- **Environment Control** — Create, edit, and manage standard or preview environments within your projects.
- **Service Orchestration** — List services, fetch specific details, and update scaling configurations on the fly.
- **Deployment Tracking** — Trigger new deployments and monitor their status in real-time.
- **Infrastructure Management** — Manage AWS account connections, VPC configurations, and environment variables.

### How it works

1. Subscribe to this server
2. Enter your Flightcontrol API Key
3. Start managing your AWS PaaS deployments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check deployment statuses and scale services without leaving the terminal or IDE.
- **Full-stack Developers** — manage staging and preview environments directly while coding.
- **Infrastructure Leads** — audit project configurations and AWS connections through simple queries.


## Available Tools (24)
- **create_aws_account_connection**: Create AWS Account Connection
- **create_cloudfront_invalidation**: Create CloudFront Cache Invalidation
- **create_deployment**: Trigger a new deployment based on repository filters
- **create_domain_group**: Create Domain Certificate Group
- **create_environment**: Create a new environment in a project
- **create_environment_variables**: Create Environment Variables
- **create_job_execution**: Trigger a one-off job in a scheduler service
- **create_project**: Automate the creation of a new project
- **create_service_variables**: Create Service Variables
- **edit_environment**: Edit an existing environment
- **edit_preview_environment**: Edit preview environment settings for a project
- **get_aws_account_details**: Get AWS Account Details
- **get_cloudfront_invalidation_status**: Get Invalidation Status
- **get_deployment_status**: Get Deployment Status
- **get_domain_details**: Get Single Domain Details
- **get_domains_from_group**: Get Domains from Group
- **get_job_execution_status**: Get Job Execution Status
- **get_service_scaling**: Get Service Scaling Information
- **get_service**: Retrieve details for a specific service
- **list_projects**: List all projects owned by the team
- **list_services**: Retrieve a paginated list of services
- **swap_blue_green**: Trigger a swap between Blue and Green environments
- **trigger_deploy_hook**: Trigger deployments via a secret URL
- **update_service_scaling**: Manually scale service instances


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flightcontrol (AWS PaaS Deployments)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our Flightcontrol projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Main-API' (ID: proj_123), 'Frontend-App' (ID: proj_456), and 'Worker-Service' (ID: proj_789). Which one would you like to inspect?

---

**👤 You:**
> "Show me the details for service ID 'srv-abc12345'."

**🤖 AI Agent:**
> Fetching service details... Service 'srv-abc12345' is a Web Service running in the 'production' environment. It is currently healthy and deployed on AWS us-east-1.

---

**👤 You:**
> "Create a new environment named 'staging' for project 'proj_123' in us-west-2."

**🤖 AI Agent:**
> Starting environment creation... I've initiated the creation of the 'staging' environment for project 'proj_123' in the us-west-2 region. I'll let you know once the configuration is ready.


## ❓ FAQ

**Q: Can I see all my active projects and their IDs?**
Yes! Use the `list_projects` tool to retrieve a complete list of projects owned by your team, including their unique identifiers and repository links.

**Q: How do I check the configuration of a specific service?**
Simply provide the Service ID to the `get_service` tool. Your agent will fetch the full details, including type, status, and current environment mapping.

**Q: Is it possible to scale my services using the AI?**
Yes, the `update_service_scaling` tool allows you to manually adjust the scaling parameters of your services directly through the conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightcontrol-aws-paas-deployments](https://vinkius.com/mcp/flightcontrol-aws-paas-deployments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flightcontrol (AWS PaaS Deployments)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flightcontrol-aws-paas-deployments` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flightcontrol (AWS PaaS Deployments)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flightcontrol-aws-paas-deployments": {
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
