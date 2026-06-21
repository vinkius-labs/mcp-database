# Cilium (eBPF Networking) MCP Server

Manage Cilium eBPF networking — inspect cluster nodes, monitor daemon health, and manage networking endpoints via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cilium-ebpf-networking)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

## Description
Connect to your **Cilium** agent to monitor and manage your Kubernetes networking stack using eBPF technology through natural language.

### What you can do

- **Cluster Visibility** — Retrieve detailed information about cluster nodes known to the local Cilium agent.
- **Health Monitoring** — Check the status of the Cilium daemon, container runtime, datastore, and Hubble connectivity.
- **Configuration Management** — Inspect and update daemon configuration options and datapath modes on the fly.
- **Endpoint Control** — List, inspect, and create networking endpoints to manage container connectivity and security.

### How it works

1. Subscribe to this server
2. Enter your Cilium API URL
3. Start managing your eBPF networking from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Platform Engineers** — quickly audit cluster health and node status without complex CLI commands
- **Security Teams** — inspect endpoint labels and states to verify network policy enforcement
- **SREs** — troubleshoot connectivity issues by querying daemon configuration and health metrics


## Available Tools
- **create_endpoint**: Create endpoint
- **get_config**: Get configuration of Cilium daemon
- **get_endpoint**: g., cilium-local:123, container-id:abc).

Get endpoint by endpoint ID
- **get_healthz**: Get health of Cilium daemon
- **get_cluster_nodes**: Get nodes information stored in the cilium-agent
- **patch_config**: Modify daemon configuration


## Installation & Usage

To install and use the **Cilium (eBPF Networking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cilium-ebpf-networking](https://vinkius.com/mcp/cilium-ebpf-networking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
