# AWS App Runner Scaling Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-app-runner-scaling-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Calculate deterministic AWS App Runner resource allocations and scaling plans.

## Description
This MCP server provides precise tools for planning AWS App Runner deployments. Use `calculate_resource_configuration` to validate vCPU and memory pairings against AWS tier constraints. Use `calculate_scaling_plan` to determine instance counts based on expected request volume and concurrency. Finally, use `generate_service_defaults` to establish operational parameters like health check intervals and ephemeral storage requirements.


## Available Tools (3)
- **calculate_resource_configuration**: Determines if a specific vCPU and Memory request is valid within AWS App Runner tier constraints
- **calculate_scaling_plan**: Calculates the required number of instances and identifies if the workload is pushing beyond recommended concurrency limits
- **generate_service_defaults**: Provides a complete set of operational parameters based on provided capacity requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS App Runner Scaling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a 0.5 vCPU and 4096 MB memory configuration valid for App Runner?"

**🤖 AI Agent:**
> Yes, a 0.5 vCPU configuration supports memory ranges from 2048 MB to 8192 MB, so 4096 MB is a valid pairing.

---

**👤 You:**
> "Calculate a scaling plan for 500 total requests with 50 requests per instance, minimum 1 and maximum 10 instances."

**🤖 AI Agent:**
> The plan requires 10 instances to handle 500 requests at 50 requests per instance.

---

**👤 You:**
> "What are the default service settings for a 5GB container image and 20GB ephemeral storage?"

**🤖 AI Agent:**
> The default settings include a 60s warm-up time, 5s health check interval, 2s timeout, and 80% CPU utilization target.


## ❓ FAQ

**Q: How do I know if my vCPU and memory selection is valid?**
You can use the `calculate_resource_configuration` tool to check if your requested vCPU and memory combination adheres to AWS App Runner's specific resource tiers.

**Q: Can I scale my App Runner service to zero?**
Yes, by using `calculate_scaling_plan` and setting the minimum instances to 0, you can plan for a scale-to-zero configuration.

**Q: What are the recommended concurrency limits?**
While there is no hard limit, it is recommended to keep concurrency per instance at or below 100 requests to maintain optimal performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-app-runner-scaling-calculator](https://vinkius.com/ai-agent-connect/aws-app-runner-scaling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS App Runner Scaling Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-app-runner-scaling-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS App Runner Scaling Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-app-runner-scaling-calculator": {
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
