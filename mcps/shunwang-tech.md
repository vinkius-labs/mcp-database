# Shunwang Tech MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shunwang-tech)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shunwang-tech-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shunwang-tech-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Leading edge computing and PC Bang management platform — monitor clusters, schedule tasks, and manage GPU resources via AI.

## Description
Empower your AI agent to orchestrate your edge computing infrastructure with **Shunwang Tech**, the dominant platform for PC Bang (Internet Cafe) management and distributed GPU resources in China. By connecting Shunwang to your agent, you transform complex resource scheduling and node monitoring into a natural conversation. Your agent can instantly list computing nodes, deploy new tasks to specific clusters, audit resource usage, and even send remote management commands without you ever touching a technical dashboard. Whether you are managing an AI inference network or a large-scale gaming infrastructure, your agent acts as a real-time infrastructure manager, ensuring your edge resources are always optimized and responsive.

### What you can do

- **Node Monitoring** — List all computing nodes in your network, check real-time metrics (CPU, GPU, RAM), and audit their health status.
- **Task Scheduling** — Create and deploy new computing tasks, stop running processes, and manage task lifecycles across your clusters.
- **Resource Optimization** — Audit overall GPU specifications and resource usage summaries to optimize your edge-cloud synergy.
- **Cluster Management** — Browse available computing clusters and organize your distributed infrastructure effectively.
- **Remote Operations** — Send management commands like reboot or shutdown to specific nodes directly through the chat interface.

### How it works

1. Subscribe to this server
2. Enter your Shunwang App Key and App Secret
3. Start managing your edge computing infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Infrastructure Engineers** — monitor and manage distributed GPU clusters and edge nodes instantly through AI.
- **AI Developers** — deploy and scale model inference tasks across Shunwang's massive edge computing network.
- **PC Bang & LAN House Owners** — oversee technical operations and client health across large networks of PCs.
- **Cloud Service Providers** — integrate Shunwang's 'Northbound' interfaces into automated resource orchestration workflows.


## Available Tools
- **create_task**: Create a new computing task
- **get_gpu_specs**: Get GPU specifications
- **get_node**: Get node details
- **get_resource_usage**: Get resource usage summary
- **list_clusters**: List computing clusters
- **list_images**: List available system images
- **list_nodes**: List all computing nodes
- **list_tasks**: List computing tasks
- **send_node_command**: Send command to node
- **stop_task**: Stop a computing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shunwang Tech** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active computing nodes in my Shunwang network."

**🤖 AI Agent:**
> I've scanned your infrastructure and found 15 active nodes. Most are running at optimal capacity, but node SW-009 is showing high GPU load. Would you like to see its details?

---

**👤 You:**
> "Deploy a new task to cluster 'Huzhou-Edge-01' using image 'ai-inference-v2'."

**🤖 AI Agent:**
> Processing deployment... Your task has been successfully created and is being deployed to cluster 'Huzhou-Edge-01'. Task ID: TSK-8821. I'll monitor its initialization for you.

---

**👤 You:**
> "What is the current GPU resource usage across my entire Shunwang infrastructure?"

**🤖 AI Agent:**
> Across your network, GPU utilization is currently at 68%. You have 120 RTX 4090 nodes available, with 45 currently dedicated to AI inference tasks. Would you like a breakdown by cluster?


## Installation & Usage

To install and use the **Shunwang Tech** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shunwang-tech](https://vinkius.com/mcp/shunwang-tech)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
