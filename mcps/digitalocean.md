# DigitalOcean MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digitalocean)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to manage cloud infrastructure, track Droplets, and monitor managed databases via the DigitalOcean API.

## Description
Integrate **DigitalOcean**, the leading cloud infrastructure provider, directly into your AI workflow. Manage your compute instances (Droplets), monitor block storage and DNS domains, track managed databases, and oversee your App Platform services using natural language.

### What you can do

- **Compute Oversight** — List and retrieve detailed configuration for all your Droplets, including IP addresses and resource status.
- **Storage & Networking** — Monitor block storage volumes and manage DNS domains directly via chat.
- **Managed Databases** — Track your database clusters (Postgres, MySQL, Redis) and their technical metadata.
- **App Platform Monitoring** — Oversee your deployed applications and their active deployment states across projects.

### How it works

1. Connect the DigitalOcean integration to your AI assistant.
2. Authorize using your DigitalOcean Personal Access Token (found in your API settings).
3. Orchestrate your cloud infrastructure and resources through intuitive conversation.

### Who is this for?

- **DevOps Engineers** — Quickly check Droplet status and network configurations on the go.
- **Cloud Architects** — Monitor resource allocation and database health via chat.
- **System Administrators** — Audit cloud projects and firewall rules during maintenance or incident response.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and limits for your DigitalOcean account
- **get_droplet_details**: Get detailed information for a specific Droplet
- **list_app_platform_services**: List all applications deployed on DigitalOcean App Platform
- **list_managed_databases**: List all managed database clusters (Postgres, MySQL, Redis, etc.)
- **list_dns_domains**: List all DNS domains managed in DigitalOcean
- **list_compute_droplets**: List all compute instances (Droplets) in your DigitalOcean account
- **list_cloud_firewalls**: List all cloud firewalls and their associated rules
- **list_cloud_projects**: List all logical projects used to group resources
- **list_block_storage_volumes**: List all block storage volumes across your account
- **search_droplets_by_name**: Search for a Droplet using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DigitalOcean** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Droplets and their IP addresses."

**🤖 AI Agent:**
> I've found 3 active Droplets: 'web-server-01' (IP: 192.168.1.10), 'db-master' (IP: 192.168.1.20), and 'worker-node' (IP: 192.168.1.30). All are currently 'Active'. Would you like to see the resource specs for db-master?

---

**👤 You:**
> "Show me our managed database clusters."

**🤖 AI Agent:**
> You have 2 managed database clusters: 'Production-Postgres' (v15, 3 nodes) and 'Staging-Redis' (v7, 1 node). Both are reported as 'Online'. Should I check the connection parameters for the production cluster?

---

**👤 You:**
> "What is the status of our App Platform services?"

**🤖 AI Agent:**
> I've retrieved 2 active services on App Platform: 'Marketing-Site' (Status: Active, Last Deploy: 2 hours ago) and 'Customer-API' (Status: Active, Last Deploy: yesterday). Would you like to see the source repositories for these apps?


## ❓ FAQ

**Q: How do I get a DigitalOcean Personal Access Token?**
Log in to your DigitalOcean account, navigate to the **API** section in the sidebar, and under the **Tokens/Keys** tab, click **Generate New Token**. Ensure you select the 'read' or 'write' scopes as needed.

**Q: Can the agent reboot a Droplet?**
This integration currently focuses on listing and auditing infrastructure resources. Power actions like rebooting or resizing should be managed via the DigitalOcean control panel or CLI.

**Q: Is the App Platform supported?**
Yes, you can use the list_app_platform_services tool to monitor your applications deployed on DigitalOcean's App Platform and check their current deployment status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digitalocean](https://vinkius.com/mcp/digitalocean)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DigitalOcean** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digitalocean` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DigitalOcean** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digitalocean": {
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
