# Vercel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vercel-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Vercel deployments, projects and domains via API — inspect builds, track deployments, manage env vars and domains from any AI agent.

## Description
Connect your **Vercel** account to any AI agent and take full control of your deployment pipeline through natural conversation.

### What you can do

- **Project Discovery** — List all projects with framework detection, git repo info and latest deployment status
- **Deployment Tracking** — View deployment history with status (READY, BUILDING, ERROR, CANCELED), URLs and git commit info
- **Deployment Management** — Get deployment details including build logs and cancel running deployments
- **Domain Management** — List and inspect custom domains with DNS records, SSL status and verification state
- **Environment Variables** — List variable keys (values hidden for security), create and delete env vars per target environment
- **Team Management** — List all teams and their associated projects
- **Runtime Logs** — Fetch deployment logs for debugging and monitoring

### How it works

1. Subscribe to this server
2. Enter your Vercel Access Token
3. Start managing your deployments from Claude, Cursor, or any MCP-compatible client

No more checking the Vercel dashboard for build status or hunting for environment variables. Your AI acts as a dedicated deployment engineer.

### Who is this for?

- **Frontend Developers** — quickly check deployment status, review build errors and manage environment variables without leaving your editor
- **DevOps Engineers** — audit deployment history, monitor domain health and track environment variable security across projects
- **Team Leads** — monitor team projects, review deployment success rates and verify domain configurations via conversation


## Available Tools (14)
- **cancel_deployment**: The deployment status will change to CANCELED. Provide the deployment ID and optionally the teamId.

Cancel a running Vercel deployment
- **create_env_var**: Requires the project ID, variable key and value. Optionally set the target environments as comma-separated values (e.g. "production,preview,development"). Returns the created variable metadata.

Create an environment variable for a Vercel project
- **delete_env_var**: Provide the project ID and the variable ID (from list_env_vars). WARNING: the variable cannot be recovered.

Delete an environment variable from a Vercel project
- **get_deployment**: Provide the deployment ID.

Get details for a specific Vercel deployment
- **get_domain**: Provide the domain name (e.g. "example.com").

Get details for a specific domain in Vercel
- **get_logs**: Optionally filter by projectId, since/until timestamps (Unix ms). Returns log entries with timestamps, messages and source. Useful for debugging deployment issues and monitoring runtime behavior.

Get runtime logs for a Vercel deployment
- **get_user**: Returns user ID, username, email, avatar and account metadata. Use this to verify your token is working correctly.

Get the authenticated Vercel user
- **get_project**: Provide the project ID (or name) and optionally the teamId.

Get details for a specific Vercel project
- **list_aliases**: Each alias maps a URL to a specific deployment. Optionally filter by teamId and projectId.

List deployment aliases (URLs) in Vercel
- **list_deployments**: Each deployment includes its ID, URL, status (READY, BUILDING, ERROR, CANCELED, INITIALIZING), creation date, git commit info and framework. Optionally filter by teamId and projectId.

List deployments for a Vercel account or project
- **list_domains**: Each domain includes its verification status, DNS records, SSL certificate status and redirect configuration. Optionally filter by teamId.

List domains configured for a Vercel team
- **list_env_vars**: Returns variable keys, target environments (production, preview, development) and types. Variable VALUES are NOT returned for security. Provide the project ID.

List environment variables for a Vercel project
- **list_projects**: Each project represents a deployed application with its own domains, environment variables and deployment history. Optionally filter by teamId. Returns project ID, name, framework, git repo and latest deployment info.

List Vercel projects
- **list_teams**: Each team has its own set of projects, deployments and members. Returns team ID, name, slug and creation date. Use the team ID as the teamId parameter in other tools.

List Vercel teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vercel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest deployments for my portfolio project."

**🤖 AI Agent:**
> I found 5 recent deployments for your portfolio project: the latest one (READY, deployed 2h ago from main branch), followed by a BUILDING deployment from 30m ago (PR #42), and an ERROR deployment from 3h ago that failed due to a build timeout.

---

**👤 You:**
> "Add the STRIPE_SECRET_KEY env var to my production environment."

**🤖 AI Agent:**
> Done! I've created the `STRIPE_SECRET_KEY` environment variable scoped to the production environment for your project. The value has been securely stored and will be available on the next deployment.

---

**👤 You:**
> "Check if my custom domain example.com is properly configured."

**🤖 AI Agent:**
> The domain example.com is VERIFIED with valid A records pointing to Vercel's IPs (76.76.21.21). SSL certificate is active and issued by Let's Encrypt. The apex domain and www subdomain are both configured correctly. No DNS misconfigurations detected.


## ❓ FAQ

**Q: How do I create a Vercel Access Token?**
Log in to the [**Vercel Dashboard**](https://vercel.com/account/tokens), go to **Settings > Access Tokens**, click **Create Token**, give it a name, select your team (optional) and scope. Copy the token immediately — it won't be shown again.

**Q: Can I manage environment variables via the agent?**
Yes! Use `list_env_vars` to see all variable keys (values are hidden for security), `create_env_var` to add new ones with key, value and target environments (production, preview, development), and `delete_env_var` to remove them.

**Q: Can I cancel a running deployment?**
Yes! Use `cancel_deployment` with the deployment ID to stop a build that is currently in progress. The deployment status will change to CANCELED. You can find the deployment ID from `list_deployments`.

**Q: How do I check my deployment history?**
Use `list_deployments` optionally filtered by teamId and projectId to see recent deployments. Each entry shows the deployment URL, status (READY, BUILDING, ERROR), framework, git commit and creation date. Use `get_deployment` with a specific deployment ID for full details including build logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vercel-alternative](https://vinkius.com/mcp/vercel-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `vercel-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vercel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vercel-alternative": {
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
