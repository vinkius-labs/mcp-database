# OceanBase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oceanbase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/oceanbase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/oceanbase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enterprise distributed relational database — manage clusters, tenants, and databases via AI.

## Description
Empower your AI agent to orchestrate your entire database infrastructure with **OceanBase**, the premier enterprise distributed relational database. By connecting OceanBase to your agent, you transform complex cluster management, tenant resource allocation, and database auditing into a natural conversation. Your agent can instantly list your database clusters, retrieve detailed configuration for tenants, monitor resource usage statistics, and browse available databases without you ever needing to navigate the OceanBase Cloud console. Whether you are conducting a capacity planning review or auditing database health across a global deployment, your agent acts as a real-time database reliability assistant, keeping your data infrastructure accurate and your systems performant.

### What you can do

- **Cluster Orchestration** — List all database clusters and retrieve detailed configuration and status information.
- **Tenant Management** — Browse logical tenants within clusters and retrieve detailed resource allocation metadata.
- **Database Auditing** — List all databases within specific tenants to identify data assets and structures.
- **Resource Monitoring** — Retrieve aggregate resource usage statistics to audit system performance and capacity.
- **Organization Insights** — Browse projects, instances, and workspaces to maintain a unified view of your database ecosystem.

### How it works

1. Subscribe to this server
2. Enter your OceanBase Access Key ID and Secret
3. Start managing your distributed database through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DBAs & Infrastructure Engineers** — automate cluster auditing and monitor resource usage through natural language queries.
- **Data Architects** — coordinate tenant strategies and audit database structures directly from your AI-powered workspace.
- **Backend Developers** — retrieve instance details and browse database catalogs via a unified AI interface.
- **OceanBase Cloud Users** — integrate your existing database workflows into your AI-driven daily routines.


## Available Tools
- **get_cluster_details**: Get cluster details
- **get_instance_details**: Get instance details
- **get_resource_stats**: Get resource statistics
- **get_tenant_details**: Get tenant details
- **get_workspaces**: Get account workspaces
- **list_clusters**: List OceanBase clusters
- **list_databases**: List tenant databases
- **list_instances**: List OB instances
- **list_projects**: List OB projects
- **list_tenants**: List cluster tenants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OceanBase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all database clusters in my OceanBase account."

**🤖 AI Agent:**
> I've retrieved your OceanBase clusters. You have 3 active clusters, including 'Prod-Cluster-01' and 'Dev-Sandbox'. Would you like to view the tenants for the production cluster?

---

**👤 You:**
> "Show me the resource usage statistics for the organization."

**🤖 AI Agent:**
> I've retrieved the resource summary. Your organization is currently using 45% of allocated CPU capacity and 62% of memory across all instances. Storage usage is stable at 1.2TB. Should I check for any tenants hitting their limits?

---

**👤 You:**
> "List all databases in tenant 'tenant-8821' inside cluster 'cluster-9920'."

**🤖 AI Agent:**
> I've retrieved the databases for the specified tenant. There are 5 logical databases, including 'InventoryDB', 'CustomerPortal', and 'AnalyticsRaw'. Would you like detailed configuration for any of them?


## Installation & Usage

To install and use the **OceanBase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oceanbase](https://vinkius.com/mcp/oceanbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
