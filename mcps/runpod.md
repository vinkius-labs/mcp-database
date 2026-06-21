# RunPod MCP Server

Integrate your AI securely to RunPod to cleanly quickly provision scalable GPU pods, manage active instances, and inspect serverless endpoints and custom templates natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/runpod)

## Overview
**Category:** superpower
**Tools Count:** 7

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


## Installation & Usage

To install and use the **RunPod** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runpod](https://vinkius.com/mcp/runpod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
