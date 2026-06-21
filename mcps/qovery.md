# Qovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qovery)
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


## ❓ FAQ

**Q: How do I securely obtain my Qovery API Token?**
Sign in to your Qovery Console. Navigate to your **Organization Settings**, then to the **API Tokens** section. Click **Generate Token** (or Add). Give it a brief name, select the desired roles, and click Create. Copy the static string immediately as it won't be shown again, and paste it to authenticate.

**Q: Can it restart specific microservices?**
Yes. Once you identify the `app_id` using the list components tools, you can instruct your agent to `restart_application`. This triggers a rolling restart exactly as if you clicked 'Restart' on the console. Traffic is routed seamlessly while pods re-initialize.

**Q: What does deploy specific Git commit do?**
Normally, Qovery auto-deploys a branch. With `deploy_application` you can force Qovery to pull a specific commit ID (SHA) and deploy it immediately to an environment. This is perfect for hotfixes, effectively circumventing prolonged CI loops while ensuring zero downtime.

**Q: Is this tool safe to run on production?**
Yes, but with caveats. Standard queries (like listing environments and getting stats) are entirely read-only. However, tools like `restart` and `deploy` are mutating operations. Always make sure you instruct your agent precisely and maintain manual approval checkpoints before executing deployment functions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qovery](https://vinkius.com/mcp/qovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qovery": {
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
