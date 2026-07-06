# Lambda Labs (GPU Cloud) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lambda-labs-gpu-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Manage AI infrastructure via Lambda Labs — launch GPU instances, monitor ML workloads, and manage SSH keys.

## Description
Connect your **Lambda Labs** account to any AI agent and take full control of your AI infrastructure and high-performance GPU orchestration through natural conversation.

### What you can do

- **Instance Orchestration** — Launch state-of-the-art GPU virtual machines (e.g., H100, A100) and manage their entire lifecycle directly from your agent
- **ML Infrastructure Audit** — List running instances and retrieve detailed hardware specifications, public IPv4 addresses, and Jupyter Lab access tokens securely
- **Inventory & Pricing** — Discover available GPU node types and pricing matrices across different regions to optimize your AI training and inference budget
- **SSH Key Management** — Enumerate globally managed public keys to ensure zero-trust infrastructure provisioning and secure access over port 22
- **Storage Mapping** — Discover persistent shared NAS volumes living in the Lambda ecosystem that can be mounted simultaneously across multiple worker nodes
- **Resource Cleanup** — Terminate and deallocate compute nodes instantly to stop billing and maintain a clean cloud footprint

### How it works

1. Subscribe to this server
2. Enter your Lambda Labs API Key
3. Start managing your GPU cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Machine Learning Engineers** — launch powerful GPU boxes for training and fine-tuning through natural conversation without manual dashboard searching
- **Data Scientists** — monitor active instances and retrieve Jupyter Lab access tokens directly from your workspace for rapid experimentation
- **AI Infrastructure Ops** — manage SSH keys and shared filesystems across multiple worker nodes to maintain scalable and secure ML environments


## Available Tools (7)
- **launch_instance**: g., powerful H100 or A100 boxes). Injects explicit SSH keys into the runtime so it is securely accessible over port 22 immediately upon boot.

Provision a new Lambda GPU virtual machine
- **terminate_instances**: Any ephemeral drives attached will be vaporized immediately without backup. Extremely destructive; stops billing instantly.

Permanently terminate and destroy Lambda GPU instances
- **list_instance_types**: Exposes exact catalog configurations of available GPU node types, identifying exactly which regions currently hold physical availability.

Discover available Lambda GPU instance specifications and pricing
- **list_ssh_keys**: Enumerate globally managed SSH public keys in Lambda
- **list_filesystems**: Map persistent shared NAS volumes living in the Lambda ecosystem
- **list_instances**: List running GPU instances on Lambda Cloud
- **get_instance**: Get exact details and SSH connection string for a specific instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lambda Labs (GPU Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my running GPU instances in Lambda Cloud"

**🤖 AI Agent:**
> I've found 2 active instances: 1) 'training-node-01' (1x H100, Region: us-east-1, Status: active), 2) 'inference-test' (1x A100, Region: us-west-1, Status: booting). Would you like the SSH connection strings for either of these?

---

**👤 You:**
> "Launch a 1x H100 instance in us-east-1 with my 'default-key' SSH key"

**🤖 AI Agent:**
> Launching GPU instance… I've triggered the provision of a 1x H100 box in us-east-1 with your 'default-key' attached. The Instance ID is 'inst-98765'. It should be ready for SSH access in approximately 2 minutes.

---

**👤 You:**
> "What are the available instance types and their current pricing?"

**🤖 AI Agent:**
> I've retrieved the latest catalog. Highlights include: gpu_1x_h100 ($2.49/hr), gpu_8x_h100 ($19.92/hr), and gpu_1x_a100_pcie ($1.10/hr). Availability is currently highest in the us-east-1 and us-south-1 regions. Would you like to check for a specific hardware setup?


## ❓ FAQ

**Q: Can I launch a high-performance H100 instance through my agent?**
Yes. Use the `launch_instance` tool and specify the type (e.g. `gpu_1x_h100`) and region. Your agent will also allow you to attach registered SSH keys so the instance is securely accessible immediately upon boot.

**Q: How do I retrieve the Jupyter Lab access token for a running node?**
Use the `get_instance` tool with your Instance ID. Your agent will fetch the complete telemetry, including the public IP and the Jupyter Lab access token if the environment is configured to provide it.

**Q: Can my agent check for GPU availability across different regions?**
Absolutely. The `list_instance_types` tool queries the cloud boundary for hardware inventory. Your agent will report which GPU node types are currently available and in which physical regions they are hosted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lambda-labs-gpu-cloud](https://vinkius.com/mcp/lambda-labs-gpu-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lambda Labs (GPU Cloud)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lambda-labs-gpu-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lambda Labs (GPU Cloud)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lambda-labs-gpu-cloud": {
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
