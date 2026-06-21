# RunPod MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runpod)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/runpod-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/runpod-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Integrate your AI securely to RunPod to cleanly quickly provision scalable GPU pods, manage active instances, and inspect serverless endpoints and custom templates natively.

## Description
Connect your AI directly to **RunPod**, the leading cloud infrastructure provider for on-demand GPU computing and serverless execution. Empower your conversational agent to act as a highly proficient DevOp engineer, managing advanced computational workloads, exploring deployment options, and spinning up new hardware instances.

### What you can do

- **Manage Pods On-Demand** — Effortlessly identify running and paused GPU machines across your cloud account (`list_pods`, `get_pod`). Halt specific billable instances to control costs securely (`stop_pod`).
- **Provision GPU Workloads** — Find verified templates or specific GPU architectures ready for deployment (`list_templates`, `list_gpu_types`), and create entirely new hardware nodes immediately directly from chat (`create_pod`).
- **Audit Serverless Environments** — Review all registered endpoints routing your containerized inference applications (`list_endpoints`).

### How it works

1. Successfully enable the RunPod orchestration integration inside your core interface.
2. Sign into your RunPod cloud console and navigate to 'Settings' > 'API Keys'. 
3. Generate a new API Key with Read/Write permissions and insert this secret inside the secure connection module below.
4. Interact seamlessly: "List all active GPU pods and point out any that are sitting idle without active usage."

### Who is this for?

- **DevOps Engineers** — Instantly provision and audit heavy workloads directly from chat interfaces without toggling through web dashboards.
- **AI Developers** — Manage high-power serverless LLM implementations organically via organic language requests.


## Available Tools
- **create_pod**: Specify name, GPU type, and Docker image.

Creates a new GPU pod
- **get_pod**: Retrieves details for a specific GPU pod
- **list_endpoints**: Lists all serverless endpoints
- **list_gpu_types**: Lists available GPU hardware types
- **list_pods**: Lists all GPU pods in the account
- **list_templates**: Lists saved pod templates
- **stop_pod**: Stops a running GPU pod


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RunPod** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our stopped GPU pods."

**🤖 AI Agent:**
> I successfully verified the RunPod platform logs. You have 2 pods currently in a paused stopped status in your configured account.

---

**👤 You:**
> "Check what GPU templates are available to deploy a new Llama-3 inference instance."

**🤖 AI Agent:**
> I have loaded the RunPod catalog template arrays. There are several pre-built images with focused PyTorch and vLLM installations tuned perfectly for Llama-3 text deployments. Would you like me to provision one specific GPU?

---

**👤 You:**
> "Pause pod with ID 'pod_xyz_980' immediately to prevent recurring costs throughout the evening."

**🤖 AI Agent:**
> Pod 'pod_xyz_980' has been carefully stopped securely. Active hourly billing operations to compute cycles for this specific cloud target are halted.


## Installation & Usage

To install and use the **RunPod** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runpod](https://vinkius.com/mcp/runpod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
