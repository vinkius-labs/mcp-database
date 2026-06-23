# Zeabur (PaaS Deployment) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zeabur-paas-deployment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deploy services, manage containers, and send transactional emails via Zeabur PaaS directly from your AI agent.

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


## Available Tools (9)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zeabur (PaaS Deployment)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Deploy a new service using this YAML template: [YAML content]"

**🤖 AI Agent:**
> I've initiated the deployment using `deploy_template`. The service is being created in your project. You can track the progress using the provided Service ID.

---

**👤 You:**
> "Get the build logs for deployment 'dep-123' in project 'proj-456'."

**🤖 AI Agent:**
> Fetching logs via `get_build_logs`... I've retrieved the build output. It seems the build failed at the 'npm install' step due to a missing dependency.

---

**👤 You:**
> "Run 'ls -la /app' in service 'srv-789' environment 'env-000'."

**🤖 AI Agent:**
> Executing command via `execute_command`... The output shows the following files in the /app directory: package.json, src, and node_modules.


## ❓ FAQ

**Q: Can I run shell commands inside my running services?**
Yes! Use the `execute_command` tool by providing the Service ID, Environment ID, and the command array (e.g., `["ls", "-la"]`). Your agent will return the output from the container.

**Q: How do I debug a failed deployment using this server?**
You can use the `get_build_logs` tool with the Project ID and Deployment ID. It will fetch the logs so your AI can analyze the errors and suggest fixes.

**Q: Does this support deploying pre-packaged ZIP files?**
Yes. First, use `create_upload_stage` to get a presigned URL and upload ID. After uploading your file, use `prepare_deployment` to trigger the actual deployment process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeabur-paas-deployment](https://vinkius.com/mcp/zeabur-paas-deployment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zeabur (PaaS Deployment)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zeabur-paas-deployment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zeabur (PaaS Deployment)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zeabur-paas-deployment": {
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
