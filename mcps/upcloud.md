# UpCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/upcloud)
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
- **assign_ip**: Provide the required assignment payload.

Assign a new IP address
- **backup_storage**: Provide the target storage UUID.

Create a storage backup
- **clone_storage**: Provide the target storage UUID.

Clone a storage
- **create_api_token**: Provide the required token configuration payload.

Create a new API token
- **create_database**: Supply the required configuration details in the body.

Create a managed database instance
- **create_firewall_rule**: Provide the server UUID and rule configuration payload.

Create a firewall rule for a server
- **create_kubernetes_cluster**: Supply the required configuration details in the body.

Create a Managed Kubernetes cluster
- **create_load_balancer**: Supply the required configuration details in the body.

Create a managed load balancer
- **create_network**: The body must define the network parameters.

Create a new SDN private network
- **create_object_storage**: Supply the required configuration details in the body.

Create a Managed Object Storage service
- **create_router**: Provide a complete JSON payload in the body.

Create a router
- **create_server**: Ensure the body contains all required parameters.

Create a new server
- **create_storage**: The body must contain all necessary details.

Create a new storage
- **delete_server**: Ensure the server UUID is correct before proceeding.

Delete a server
- **export_audit_logs**: Export account audit logs
- **get_account**: Get UpCloud account information
- **get_billing_summary**: Get monthly billing summary
- **get_host**: Provide a valid host ID for the query.

Get host details
- **get_kubernetes_kubeconfig**: Use the cluster UUID.

Get Kubernetes cluster credentials (kubeconfig)
- **get_server**: Use the server’s unique UUID.

Get detailed server information
- **import_storage**: Provide the target storage UUID.

Import data to storage
- **list_api_tokens**: List API tokens
- **list_audit_logs**: List account audit logs
- **list_databases**: List managed database services
- **list_database_types**: List available database types and plans
- **list_firewall_rules**: Provide the server UUID.

List firewall rules for a server
- **list_hosts**: List available hosts
- **list_ips**: List all IP addresses
- **list_kubernetes_clusters**: List Managed Kubernetes (UKS) clusters
- **list_load_balancers**: List managed load balancer services
- **list_networks**: List all SDN private networks
- **list_object_storages**: List Managed Object Storage services
- **list_prices**: List resource prices
- **list_routers**: List routers
- **list_servers**: List all servers
- **list_storages**: List all accessible storages
- **list_zones**: List available zones
- **release_ip**: Provide the IP address to be released.

Release an IP address
- **restart_server**: Provide the unique server UUID.

Restart a server
- **restore_storage**: Provide the UUID of the storage.

Restore storage from backup
- **start_server**: Provide the unique server UUID.

Start a server
- **stop_server**: Provide the unique server UUID.

Stop a server
- **update_ip**: Specify the IP address and update payload.

Modify PTR record or floating IP attachment
- **update_network**: Provide the network UUID and update payload.

Modify network details
- **update_server**: Supply both the server UUID and the update payload.

Modify server configuration
- **update_storage**: The UUID must identify the target storage.

Modify or resize storage


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

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/upcloud](https://vinkius.com/en/ai-agent-connect/upcloud)
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
