# Cilium (eBPF Networking) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cilium-ebpf-networking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cilium-ebpf-networking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cilium-ebpf-networking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Cilium eBPF networking — inspect cluster nodes, monitor daemon health, and manage networking endpoints via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cilium (eBPF Networking)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the health status of the Cilium daemon."

**🤖 AI Agent:**
> I've checked the Cilium health status. The daemon is healthy, with active connectivity to Kubernetes and Hubble. Container runtime status is also green.

---

**👤 You:**
> "List all cluster nodes known to the agent."

**🤖 AI Agent:**
> I've retrieved the cluster nodes. I found 3 nodes: 'node-1' (10.0.0.1), 'node-2' (10.0.0.2), and 'node-3' (10.0.0.3). All are currently reachable.

---

**👤 You:**
> "Get the details for endpoint ID cilium-local:123."

**🤖 AI Agent:**
> Inspecting endpoint 'cilium-local:123'... It is in 'ready' state, assigned IP 10.244.1.5, and carries labels like 'app=frontend'.


## Installation & Usage

To install and use the **Cilium (eBPF Networking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cilium-ebpf-networking](https://vinkius.com/mcp/cilium-ebpf-networking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
