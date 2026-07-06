# UpCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage UpCloud infrastructure via AI — control servers, monitor billing, and manage storage across global zones directly from your agent.

## Description
Connect your **UpCloud** account to any AI agent to manage your high-performance cloud infrastructure through natural language. From deploying servers to monitoring resource costs, take full control of your cloud environment.

### What you can do

- **Server Control** — List, create, start, stop, and restart cloud servers across all global regions.
- **Storage Management** — List, create, modify, and clone storage resources to scale your data needs.
- **Infrastructure Insights** — Query available zones and physical hosts to optimize your deployment strategy.
- **Account & Billing** — Monitor your account limits, credits, and detailed monthly billing summaries.
- **Pricing Transparency** — Instantly list resource prices in your account's currency to manage cloud spend.

### How it works

1. Subscribe to this server
2. Enter your UpCloud API credentials
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to check server statuses or billing cycles. Your AI acts as a dedicated cloud architect and DevOps assistant.

### Who is this for?

- **DevOps Engineers** — automate server lifecycle management and infrastructure audits without leaving the terminal or IDE.
- **Cloud Architects** — quickly query zone availability and host details to plan high-availability setups.
- **Finance & Ops** — retrieve billing summaries and resource prices to maintain budget control over cloud environments.


## Available Tools (46)
- **get_billing_summary**: Get monthly billing summary
- **clone_storage**: Clone a storage
- **create_database**: Create a managed database instance
- **create_firewall_rule**: Create a firewall rule for a server
- **create_kubernetes_cluster**: Create a Managed Kubernetes cluster
- **create_load_balancer**: Create a managed load balancer
- **create_network**: Create a new SDN private network
- **create_object_storage**: Create a Managed Object Storage service
- **create_router**: Create a router
- **create_server**: Create a new server
- **create_storage**: Create a new storage
- **create_api_token**: Create a new API token
- **list_database_types**: List available database types and plans
- **list_databases**: List managed database services
- **delete_server**: Delete a server
- **export_audit_logs**: Export account audit logs
- **list_firewall_rules**: List firewall rules for a server
- **get_server**: Get detailed server information
- **get_host**: Get host details
- **list_hosts**: List available hosts
- **import_storage**: Import data to storage
- **list_ips**: List all IP addresses
- **get_kubernetes_kubeconfig**: Get Kubernetes cluster credentials (kubeconfig)
- **list_kubernetes_clusters**: List Managed Kubernetes (UKS) clusters
- **list_load_balancers**: List managed load balancer services
- **list_networks**: List all SDN private networks
- **list_object_storages**: List Managed Object Storage services
- **list_prices**: List resource prices
- **release_ip**: Release an IP address
- **restart_server**: Restart a server
- **restore_storage**: Restore storage from backup
- **list_routers**: List routers
- **list_servers**: List all servers
- **start_server**: Start a server
- **stop_server**: Stop a server
- **list_storages**: List all accessible storages
- **list_api_tokens**: List API tokens
- **update_ip**: Modify PTR record or floating IP attachment
- **update_network**: Modify network details
- **update_server**: Modify server configuration
- **update_storage**: Modify or resize storage
- **list_zones**: List available zones
- **get_account**: Get UpCloud account information
- **backup_storage**: Create a storage backup
- **assign_ip**: Assign a new IP address
- **list_audit_logs**: List account audit logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UpCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my UpCloud account information and credits."

**🤖 AI Agent:**
> I've retrieved your account details. You currently have $150.00 in credits remaining, and your resource limits allow for up to 20 concurrent servers. Would you like to see your billing summary for this month?

---

**👤 You:**
> "List all my active servers on UpCloud."

**🤖 AI Agent:**
> Fetching your server list... I found 3 servers: 'web-prod-01' (Running), 'db-master' (Running), and 'test-bench' (Stopped). Which one would you like to manage?

---

**👤 You:**
> "Restart the server with UUID 00264663-890e-473c-9189-9e87483660c2."

**🤖 AI Agent:**
> Initiating restart for server 00264663-890e-473c-9189-9e87483660c2... The command has been sent successfully. The server should be back online in a few moments.


## ❓ FAQ

**Q: Can I check my current account balance and resource limits?**
Yes! Use the `get_account` tool to retrieve your current credits and resource limits directly from your UpCloud account.

**Q: How do I see which global locations are available for deployment?**
Simply ask the agent to run the `list_zones` action. It will provide a complete list of physical sites where you can deploy your infrastructure.

**Q: Is it possible to restart a server using its ID?**
Yes. By providing the server's UUID to the `restart_server` tool, your AI agent can trigger a reboot of that specific instance immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upcloud](https://vinkius.com/mcp/upcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UpCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UpCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upcloud": {
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
