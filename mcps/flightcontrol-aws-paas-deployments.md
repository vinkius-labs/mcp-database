# Flightcontrol (AWS PaaS Deployments) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flightcontrol-aws-paas-deployments)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flightcontrol-aws-paas-deployments-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flightcontrol-aws-paas-deployments-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Flightcontrol (AWS PaaS Deployments)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightcontrol-aws-paas-deployments](https://vinkius.com/mcp/flightcontrol-aws-paas-deployments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
