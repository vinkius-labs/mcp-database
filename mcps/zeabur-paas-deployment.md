# Zeabur (PaaS Deployment) MCP Server

Deploy services, manage containers, and send transactional emails via Zeabur PaaS directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zeabur-paas-deployment)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Zeabur** account to any AI agent to automate your cloud infrastructure and deployment workflows through natural conversation.

### What you can do

- **Template Deployment** — Deploy new services using raw YAML specifications directly to your projects.
- **Container Management** — Execute shell commands inside service containers or download specific files for inspection.
- **Observability** — Fetch real-time build logs to debug deployment issues without leaving your chat interface.
- **ZIP Deployments** — Handle the full lifecycle of pre-packaged application deployments, from creating upload stages to final preparation.
- **Transactional Email** — Send single or batch personalized emails using the Zeabur Email REST API infrastructure.

### How it works

1. Subscribe to this server
2. Enter your Zeabur API Token (and optionally your Email Token)
3. Start managing your PaaS resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate service scaling, command execution, and environment management.
- **Full-stack Developers** — deploy templates and check build logs directly from the code editor.
- **Backend Teams** — integrate transactional email sending and container file management into automated workflows.


## Available Tools
- **create_upload_stage**: Create an upload stage for deploying pre-packaged applications
- **deploy_template**: Deploy a service using a template specification YAML
- **download_file**: Download a file from a service container
- **execute_command**: Run a command within a service container
- **get_build_logs**: Retrieve build logs for a deployment
- **prepare_deployment**: Prepare a deployment after uploading a file
- **schedule_email**: Requires ZEABUR_EMAIL_TOKEN.

Schedule an email to be sent later via Zeabur Email
- **send_batch_emails**: Requires ZEABUR_EMAIL_TOKEN.

Send batch personalized emails via Zeabur Email
- **send_email**: Requires ZEABUR_EMAIL_TOKEN.

Send a single transactional email via Zeabur Email


## Installation & Usage

To install and use the **Zeabur (PaaS Deployment)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeabur-paas-deployment](https://vinkius.com/mcp/zeabur-paas-deployment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
