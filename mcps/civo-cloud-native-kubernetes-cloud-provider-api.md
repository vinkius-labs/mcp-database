# Civo (Cloud-native Kubernetes Cloud Provider API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Civo cloud infrastructure — provision Kubernetes clusters, control compute instances, and monitor usage directly via AI.

## Description
Connect your **Civo** account to any AI agent to manage your cloud-native infrastructure through natural language. This server provides full access to Civo's high-performance K3s and compute services.

### What you can do

- **Kubernetes Management** — Create, list, and recycle nodes in K3s clusters across multiple regions using `create_cluster` and `list_clusters`.
- **Compute Instances** — Launch, reboot, stop, and resize virtual machines with tools like `create_instance` and `resize_instance`.
- **Networking & Security** — Configure private networks and firewalls with `create_network` and `create_firewall_rule`.
- **Storage & Domains** — Manage block storage volumes and DNS records with `create_volume` and `create_domain_record`.
- **Account Insights** — Monitor your resource limits and billing in real-time using `get_quota` and `get_charges`.

### How it works

1. Subscribe to this server
2. Enter your Civo API Key
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Automate cluster provisioning and scaling without leaving the terminal or chat interface.
- **Developers** — Quickly spin up dev environments or instances for testing directly from your IDE.
- **SREs** — Monitor quotas and manage firewall rules through simple conversational commands.


## Available Tools (33)
- **create_cluster**: Create a new Kubernetes cluster
- **create_domain**: Create a DNS domain
- **create_firewall_rule**: Create a firewall rule
- **create_firewall**: Create a firewall
- **create_instance**: Create a new compute instance
- **create_network**: Create a private network
- **create_team**: Create a team
- **create_volume**: Create a volume
- **create_webhook**: Create a webhook
- **detach_volume**: Detach a volume
- **get_charges**: Get hourly usage report for chargeable resources
- **list_clusters**: List Kubernetes clusters
- **list_disk_images**: List disk images
- **list_domains**: List DNS domains
- **list_firewall_rules**: List rules for a firewall
- **list_networks**: List private networks
- **list_regions**: List available regions
- **list_sizes**: List available instance sizes
- **reboot_instance**: Hard reboot an instance
- **recycle_cluster_node**: Recycle a node in a Kubernetes cluster
- **resize_instance**: Upgrade or resize an instance
- **retag_instance**: Retag an instance
- **soft_reboot_instance**: Soft reboot an instance
- **start_instance**: Start an instance
- **stop_instance**: Stop an instance
- **test_webhook**: Test a webhook
- **update_team_member_status**: Update team member status
- **upload_ssh_key**: Upload an SSH key
- **add_team_member**: Add a member to a team
- **attach_volume**: Attach a volume to an instance
- **create_domain_record**: Create a DNS record
- **get_quota**: Get account quota and usage
- **list_ssh_keys**: List SSH keys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Civo (Cloud-native Kubernetes Cloud Provider API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Kubernetes clusters in the lon1 region."

**🤖 AI Agent:**
> I've retrieved your clusters in lon1. You have one active cluster: 'production-k3s' (ID: 8f2d...) with 3 nodes currently running.

---

**👤 You:**
> "Create a new g3.xsmall instance named 'web-server' in my default network."

**🤖 AI Agent:**
> Starting the provisioning process for 'web-server' (size: g3.xsmall). I'll use your default network ID. The instance is being created now.

---

**👤 You:**
> "What is my current account quota and total charges for this month?"

**🤖 AI Agent:**
> Your current quota shows 8/10 instances used and 24/40 CPU cores. Your estimated charges for this billing cycle are $42.50.


## ❓ FAQ

**Q: Can I create a Kubernetes cluster in a specific region?**
Yes, you can use the `create_cluster` tool and specify the `region` parameter (e.g., 'lon1' or 'nyc1') along with the cluster name and network ID.

**Q: How do I restart a stuck compute instance?**
You can use the `reboot_instance` tool for a hard reboot or `soft_reboot_instance` for a graceful restart by providing the Instance ID.

**Q: Can I check my current cloud spending and limits?**
Absolutely. Use the `get_charges` tool to see your current billing details and `get_quota` to check your account resource limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api](https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Civo (Cloud-native Kubernetes Cloud Provider API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `civo-cloud-native-kubernetes-cloud-provider-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Civo (Cloud-native Kubernetes Cloud Provider API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "civo-cloud-native-kubernetes-cloud-provider-api": {
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
