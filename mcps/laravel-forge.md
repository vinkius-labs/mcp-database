# Laravel Forge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/laravel-forge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Laravel Forge servers, orchestrate site deployments, and query databases directly from your AI agent.

## Description
Connect your **Laravel Forge** developer account to an AI agent to execute complex devops tasks natively in chat.

### What you can do

- **Server Ecosystems** — List all connected drops, inspect internal structures, and check status
- **Deployments** — Safely dispatch site deployment scripts and watch output structures
- **Database Configurations** — Query connected DB clusters linked to given domains
- **Worker Operations** — Expose active daemon configurations routing jobs under your servers

### How it works

1. Subscribe dynamically to this endpoint
2. Provide your core Laravel Forge API token string
3. Engage your new devops engineer via Cursor or Claude

### Who is this for?

- **DevOps Engineers** — run deployments natively through chat commands during sprint reviews
- **Lead Developers** — instantly check worker and SSH key metadata safely tracked inside Forge environments
- **System Admins** — audit entire physical networks executing zero shell scripts


## Available Tools (9)
- **get_site**: Look up specifics for an exact site layout on a server
- **list_databases**: List active databases mounted on a Forge server
- **list_recipes**: Retrieve available custom shell recipes within your organizational team limits
- **list_servers**: Retrieve the master list of all connected Forge servers
- **list_sites**: List websites mounted to a specific server
- **list_ssh_keys**: Retrieve active physical access keys inserted on the root server
- **list_workers**: Retrieve queue worker configurations executing on a tracked site
- **deploy_site**: Command a deployment script queue to execute on a repository site
- **get_server**: Retrieve detailed data on a specific server droplet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laravel Forge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Display all the cloud server instances operating in the fleet."

**🤖 AI Agent:**
> Here's what I observed... You have 2 droplets attached: 'Production Web' and 'Staging Loadbalancer'. Should I probe their sites?

---

**👤 You:**
> "Deploy the pending commits directly to staging site 5210 on server 1205."

**🤖 AI Agent:**
> Deploying package payload... Success! Forge emitted a validation flag kicking off the repository deployment routine on site 5210.

---

**👤 You:**
> "Check the active workers running on the production server."

**🤖 AI Agent:**
> Scanning worker processes... Found 2 active Queue workers on the Production Server handling redis payloads securely.


## ❓ FAQ

**Q: How do I get started?**
Subscribe, copy your active API Token (which you generate inside **Forge Dashboard → API**), and connect it. The integration expects standard connections so you can trigger real build routines natively without intricate pipelines or ssh logic.

**Q: Can my AI automatically trigger site deployments?**
Yes! Give the agent the Server ID and Site ID you're questioning. It utilizes `deploy_site` to physically POST to Forge's pipelines kicking off an automated release. Perfect for hands-free releases right from Cursor.

**Q: What happens when I want to fetch metrics on queued application workers?**
Provide the exact IDs. The tool evaluates endpoint rules (`list_workers`) and unpacks default configurations running PHP queues natively back to the terminal screen.

**Q: Does it list physical server setups efficiently?**
Absolutely. Execute 'list_servers' or probe 'list_ssh_keys'. It aggregates root connection statuses, IPs, and structural records giving immense monitoring peace-of-mind at the keyboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/laravel-forge](https://vinkius.com/mcp/laravel-forge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laravel Forge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `laravel-forge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laravel Forge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laravel-forge": {
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
