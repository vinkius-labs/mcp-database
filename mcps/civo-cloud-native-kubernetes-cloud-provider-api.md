# Civo (Cloud-native Kubernetes Cloud Provider API) MCP Server

Manage Civo cloud infrastructure — provision Kubernetes clusters, control compute instances, and monitor usage directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api)

## Overview
**Category:** developer-tools
**Tools Count:** 33

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


## Available Tools
- **add_team_member**: Add a member to a team
- **attach_volume**: Attach a volume to an instance
- **create_cluster**: Create a new Kubernetes cluster
- **create_domain_record**: Create a DNS record
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
- **get_quota**: Get account quota and usage
- **list_clusters**: List Kubernetes clusters
- **list_disk_images**: List disk images
- **list_domains**: List DNS domains
- **list_firewall_rules**: List rules for a firewall
- **list_networks**: List private networks
- **list_regions**: List available regions
- **list_sizes**: List available instance sizes
- **list_ssh_keys**: List SSH keys
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


## Installation & Usage

To install and use the **Civo (Cloud-native Kubernetes Cloud Provider API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api](https://vinkius.com/mcp/civo-cloud-native-kubernetes-cloud-provider-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
