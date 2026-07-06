# Vercel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vercel-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Deploy frontend applications instantly with a platform optimized for Next.js, serverless functions, and edge computing globally.

## Description
Connect your **Vercel** account to any AI agent and simplify how you manage your cloud infrastructure, frontend deployments, and serverless projects through natural conversation.

### What you can do

- **Project Management** — List all projects in your account or team and retrieve detailed configuration metadata.
- **Deployment Control** — Track build history, check deployment status (READY, ERROR, BUILDING), and trigger new builds or delete old records.
- **Domain Configuration** — List all registered domains and link custom domains to specific projects instantly.
- **ENV Management** — List and create environment variables for your projects to manage secrets and configurations safely.
- **Team Visibility** — Query accessible teams and retrieve your user profile details to understand your permissions.

### How it works

1. Subscribe to this server
2. Enter your Vercel Access Token (found in your account settings under Tokens)
3. Start managing your cloud ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly check deployment health and manage environment variables via simple AI commands.
- **Frontend Developers** — monitor build status and verify domain configurations during the development cycle.
- **Product Owners** — get instant bird's-eye views of project history and deployment progress without leaving the workspace.


## Available Tools (11)
- **get_vercel_project_details**: Get details for a specific project
- **get_vercel_user_profile**: Get current user profile
- **list_vercel_deployments**: List recent deployments
- **list_vercel_account_domains**: List all account domains
- **list_vercel_project_env_vars**: List environment variables
- **list_vercel_projects**: List all Vercel projects
- **list_vercel_teams**: List accessible Vercel teams
- **add_vercel_environment_variable**: Add a new environment variable
- **create_vercel_deployment**: Create a new deployment
- **delete_vercel_deployment**: Delete a specific deployment
- **get_vercel_deployment_info**: Get details for a specific deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vercel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Vercel team."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to: 'vinkius-app', 'marketing-blog', and 'api-gateway'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the status of the latest deployment for 'vinkius-app'."

**🤖 AI Agent:**
> The latest deployment for 'vinkius-app' (ID: dpl_8823...) is currently in 'READY' state. It was deployed successfully to vinkius-app.vercel.app.

---

**👤 You:**
> "Add the environment variable 'DB_PASSWORD' to the project 'api-gateway'."

**🤖 AI Agent:**
> Success! I've added 'DB_PASSWORD' to 'api-gateway'. The change is now active for production, preview, and development environments.


## ❓ FAQ

**Q: Can I see if a specific deployment failed using the AI?**
Yes! Use the `get_deployment_info` tool with the Deployment ID. Your agent will retrieve the current state, and if it's 'ERROR', it will show you the deployment details.

**Q: How do I add a new API Key to a project via AI?**
Use the `add_environment_variable` action. Provide the project name/ID, the key name, and the value. You can also specify the type as 'secret' or 'sensitive'.

**Q: Is it possible to list all domains linked to my account?**
Absolutely. Use the `list_account_domains` query to retrieve a complete list of all domains registered or configured within your Vercel account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vercel-extended](https://vinkius.com/mcp/vercel-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vercel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vercel-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vercel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vercel-extended": {
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
