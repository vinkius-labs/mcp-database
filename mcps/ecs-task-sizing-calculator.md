# ECS Task Sizing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ecs-task-sizing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate precise AWS ECS task resources, EC2 capacity, and scaling configurations.

## Description
This MCP server provides deterministic calculations for AWS ECS resource planning. Use `calculate_task_resources` to determine exact CPU and memory requirements for Fargate and EC2, including mandatory overhead. Use `plan_ec2_capacity` to calculate how many tasks fit on a specific EC2 instance, and `evaluate_service_configuration` to plan for Cloud Map service discovery and target tracking scaling.


## Available Tools (3)
- **calculate_task_resources**: 
- **evaluate_service_configuration**: Evaluate service discovery and scaling
- **plan_ec2_capacity**: Calculate tasks per EC2 instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECS Task Sizing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate resources for a Fargate task with 2 containers, each needing 512MB memory and 256 CPU units."

**🤖 AI Agent:**
> The total CPU required is 512 units and the total memory required is 1024 MB. This combination is valid for Fargate.

---

**👤 You:**
> "How many tasks can I run on an EC2 instance with 8192 MB of memory if each task needs 1024 MB?"

**🤖 AI Agent:**
> You can run 7 tasks on this EC2 instance. (8192 MB total / 1280 MB per task including overhead).

---

**👤 You:**
> "Evaluate service configuration for a service using Cloud Map with a 70% target utilization."

**🤖 AI Agent:**
> Service discovery via Cloud Map will add operational overhead. The scaling metric to track is ECSServiceAutoScalingTargetTrackingUtilization with a target value of 70.


## ❓ FAQ

**Q: How does the tool handle EC2 overhead?**
For EC2 launch types, the tool automatically adds a 256 MB memory overhead to the total task size to account for the ECS agent and system processes.

**Q: Can I validate Fargate CPU and memory combinations?**
Yes, the `calculate_task_resources` tool validates your requested CPU and memory against official AWS Fargate constraints and flags invalid combinations.

**Q: How many tasks can I fit on my EC2 instance?**
You can use the `plan_ec2_capacity` tool by providing the total task memory and the instance memory to get the maximum number of tasks per instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ecs-task-sizing-calculator](https://vinkius.com/ai-agent-connect/ecs-task-sizing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ECS Task Sizing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ecs-task-sizing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ECS Task Sizing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecs-task-sizing-calculator": {
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
