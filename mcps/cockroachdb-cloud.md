# CockroachDB Cloud MCP Server

Manage distributed SQL clusters via CockroachDB Cloud — track clusters, monitor nodes, and audit network allowlists directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cockroachdb-cloud)

## Overview
**Category:** fort-knox
**Tools Count:** 8

## Description
Connect your **CockroachDB Cloud** account to any AI agent and take full control of your distributed SQL infrastructure through natural conversation. Streamline how you monitor and manage your globally-scalable databases natively.

### What you can do

- **Cluster Oversight** — List and retrieve details for all CockroachDB Cloud clusters including provider and region info natively
- **Node Intelligence** — Access and monitor individual nodes within your clusters to understand health and status flawlessly
- **Operation Auditing** — List and review recent management operations like scaling or upgrades to track changes securely
- **Network Logistics** — Access and monitor network allowlist rules to ensure secure database connectivity flawlessly
- **Encryption Management** — List Customer Managed Keys (CMKs) used for cluster-level data encryption flawlessly
- **Account Visibility** — Retrieve information about your authenticated user profile and organization directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CockroachDB Cloud API Secret Key
3. Start managing your distributed databases from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Database Administrators (DBAs)** — monitor cluster health and operation history using natural language
- **Cloud Engineers** — audit network allowlists and regional distribution without opening the cloud console
- **Security Teams** — quickly look up encryption key metadata and connectivity rules straight from their chat interface
- **Platform Teams** — verify cloud provider availability and monitor cluster lifecycle events


## Available Tools
- **get_cluster_cloud_details**: Get detailed information for a specific cluster
- **get_my_cockroach_profile**: Retrieve information about the authenticated user/organization
- **list_network_allowlist**: List network allowlist rules for a specific cluster
- **list_encryption_keys**: List Customer Managed Keys (CMKs) used for cluster encryption
- **list_supported_cloud_providers**: List cloud providers supported by CockroachDB Cloud
- **list_cockroach_clusters**: List all CockroachDB Cloud clusters
- **list_cluster_nodes**: List all nodes within a specific cluster
- **list_cluster_operations**: List recent management operations for a cluster (e.g. scaling, upgrades)


## Installation & Usage

To install and use the **CockroachDB Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cockroachdb-cloud](https://vinkius.com/mcp/cockroachdb-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
