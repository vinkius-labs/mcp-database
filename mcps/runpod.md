# RunPod MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runpod)
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


## Available Tools (7)
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


## ❓ FAQ

**Q: Can the AI forcefully terminate or delete critical production endpoint fleets on demand?**
No. This module safely allows the AI to only pause and manage running instances. Destructive deletion actions (like completely erasing a pod) are intentionally prohibited by the tooling design to protect your critical compute resources from unintended loss.

**Q: Can the AI provision large GPU arrays automatically?**
Yes. Using the `create_pod` capability, the AI can query the available hardware models (such as A100 or H100) and immediately launch new Docker clusters based on existing community templates, simplifying complex DevOps scaling actions significantly.

**Q: Will the AI know the billing state or the real-time cost of running each endpoint?**
No. The current RunPod AI module is concentrated on operational control and system orchestration, such as discovering inactive processes and booting new instances. Deep billing analytics or invoice extraction is not natively integrated in the commands exposed to the AI at this time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runpod](https://vinkius.com/mcp/runpod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RunPod** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runpod` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RunPod** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runpod": {
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
