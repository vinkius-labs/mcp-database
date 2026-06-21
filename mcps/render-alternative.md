# Render MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/render-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Automate your PaaS infrastructure via Render — list your services, deploy code, check logs, and scale resources directly from any AI agent.

## Description
Connect your **Render** organizational account to any AI agent and command your edge infrastructure seamlessly through natural conversation.

### What you can do

- **Service Explorer** — Query your entire portfolio of microservices, static sites, web services, and databases.
- **Deployments** — Safely trigger standard or 'Clear Cache' deploys targeting specific services via ID.
- **Scale & Operation** — Scale horizontal instances or instantly suspend/resume background workers.
- **Network Config** — Verify your custom domains and retrieve hidden environment variables deployed directly in your edge environments.

### How it works

1. Subscribe to this server
2. Enter your Render API Key
3. Manage your cloud platform deployments directly from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **DevOps Engineers** — Handle scaling rules and routine deploy checks from their terminal without surfing dashboard UIs.
- **Full-Stack Developers** — Fetch staging environment variables on the fly while actively coding.
- **Incident Responders** — Swiftly list and verify active deployment logs to remediate downtime states natively.


## Available Tools
- **create_deploy**: Trigger a new deploy for a service
- **get_service**: Get a single Render service details
- **list_custom_domains**: List custom domains for a service
- **list_deploys**: List deploys for a service
- **list_env_vars**: List environment variables for a service
- **list_services**: List Render services
- **resume_service**: Resume a suspended Render service
- **scale_service**: Only applies to services that support horizontal scaling.

Scale a Render service
- **suspend_service**: Suspend a Render service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Render** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all running backend and logic services on my Render account."

**🤖 AI Agent:**
> I've pulled the core array. You have 3 primary services active: 'Vinkius-Engine' (srv-124, running Postgres), 'Core-API' (srv-239, running Node), and 'Static-Landing' (srv-884, running Next.js). Shall we scale the Core API?

---

**👤 You:**
> "My recent deploy on the API just failed. Start a fresh deploy now and clear the cache."

**🤖 AI Agent:**
> Understood. Firing deploy sequence for Service ID `srv-239`. The clear cache flag has been successfully appended. Deploy `dep-ab294c` has been initialized and is transitioning into 'build' phase.

---

**👤 You:**
> "Scale our main API worker down to zero instances temporarily to cut costs for the weekend."

**🤖 AI Agent:**
> Action dispatched logically. Scaling service `srv-workers-8a` down to `0` instances. Operations have halted on the target. Let me know when you desire to reinstate operations.


## ❓ FAQ

**Q: Can I suspend a running worker to save money?**
Absolutely. You can execute `suspend_service` passing the specific Service ID (e.g. `srv-xyz`). The target resource will immediately enter the suspended state.

**Q: If a deploy fails, can I instruct the agent to re-deploy without using previous cache files?**
Yes! The `create_deploy` tool specifically maps a `clearCache` parameter. Telling your agent to 'deploy without cache' will map it appropriately, guaranteeing a clean build layer from your repository.

**Q: How do I easily extract the full list of Secrets / Environment variables for local parity?**
Run `list_env_vars` for your backend service. It will return all key-value mappings perfectly, allowing you to instantly align your local `.env` with production secrets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/render-alternative](https://vinkius.com/mcp/render-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Render** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `render-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Render** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "render-alternative": {
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
