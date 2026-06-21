# Linode (Akamai) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linode-akamai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/linode-akamai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/linode-akamai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Linode cloud infrastructure—provision compute instances, manage Kubernetes clusters (LKE), and monitor account details directly from your AI agent.

## Description
Connect your **Linode (Akamai)** account to any AI agent to manage your cloud infrastructure through natural language. This server provides comprehensive tools for compute and container orchestration.

### What you can do

- **Compute Management** — List, create, view, update, and delete Linode instances (VPS) across global regions using `list_linodes` and `create_linode`.
- **Kubernetes (LKE)** — Deploy and manage Linode Kubernetes Engine clusters, including node pool configuration via `create_lke_cluster`.
- **Account Oversight** — Retrieve account details and list authorized users with `get_account` and `list_users` to maintain security and visibility.
- **Instance Control** — Provision servers with specific images (like Ubuntu 22.04) and hardware types instantly.

### How it works

1. Subscribe to this server
2. Enter your Linode Personal Access Token
3. Start managing your cloud resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check cluster statuses or spin up temporary environments without leaving the terminal or IDE.
- **Full-stack Developers** — manage backend infrastructure directly from the code editor while building applications.
- **Cloud Architects** — audit account resources and user access through conversational queries.


## Available Tools
- **create_linode**: Create a new Linode
- **create_lke_cluster**: Create an LKE Cluster
- **delete_linode**: Delete a Linode
- **get_account**: View Account Details
- **get_linode**: View a specific Linode
- **get_lke_cluster**: View an LKE Cluster
- **list_linodes**: List all Linodes (Compute Instances)
- **list_lke_clusters**: List LKE Clusters
- **list_users**: Manage Users
- **update_linode**: Update a Linode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linode (Akamai)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Linode instances."

**🤖 AI Agent:**
> I've retrieved your Linodes. You have 3 active instances: 'web-server-prod' (ID: 12345) in us-east, 'db-master' (ID: 12346) in eu-central, and 'staging-app' (ID: 12347) in ap-south.

---

**👤 You:**
> "Create a new g6-standard-1 Linode in the us-east region with Ubuntu 22.04."

**🤖 AI Agent:**
> Provisioning your new Linode... The instance has been created with ID 54321. It is currently booting in the us-east region with Ubuntu 22.04 LTS.

---

**👤 You:**
> "Show me the details of my Kubernetes clusters."

**🤖 AI Agent:**
> Fetching LKE clusters... I found one cluster: 'production-cluster' (ID: 9876). It's running K8s version 1.25 in us-east with 3 nodes in the default pool.


## Installation & Usage

To install and use the **Linode (Akamai)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linode-akamai](https://vinkius.com/mcp/linode-akamai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
