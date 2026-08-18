# AWS CloudFormation Stack Limits Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-cloudformation-stack-limits-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Verify AWS CloudFormation template compliance and calculate stack limits.

## Description
This MCP server provides deterministic calculations for AWS CloudFormation service quotas. Use `check_template_compliance` to verify if your template size and resource count stay within AWS limits. Use `calculate_stack_capacities` to find maximum allowed outputs and parameters. You can also use `evaluate_stack_set_limits` for multi-account deployment planning and `assess_deployment_health` to check for recommended nested stack depth and change set counts.


## Available Tools (4)
- **assess_deployment_health**: Provides recommendations on nested depth and change set management to ensure deployment stability
- **calculate_stack_capacities**: Calculates specific limits for parameters, outputs, and policies based on standard stack constraints
- **check_template_compliance**: Determines if a provided template configuration stays within standard AWS service quotas
- **evaluate_stack_set_limits**: Calculates limits for multi-account deployments using Stack Sets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS CloudFormation Stack Limits Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my CloudFormation template with 600 resources compliant?"

**🤖 AI Agent:**
> The template is not compliant. It exceeds the standard 500 resource limit, though it may be acceptable if you have an account quota increase.

---

**👤 You:**
> "What is the maximum number of parameters I can have in a stack?"

**🤖 AI Agent:**
> The maximum number of parameters allowed per stack is 200.

---

**👤 You:**
> "I have a nested stack depth of 7. Is this a problem?"

**🤖 AI Agent:**
> Yes, a nesting depth of 7 exceeds the recommended limit of 5 to avoid complexity and circular dependencies.


## ❓ FAQ

**Q: How do I check if my template exceeds AWS resource limits?**
You can use the `check_template_compliance` tool by providing your template size in KB and the total resource count.

**Q: What are the standard limits for stack outputs and parameters?**
The standard limit for both outputs and parameters is 200 per stack. You can verify this using `calculate_stack_capacities`.

**Q: Can I check limits for Stack Sets?**
Yes, use the `evaluate_stack_set_limits` tool to determine the maximum number of stack sets and instances per set allowed for your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-cloudformation-stack-limits-calculator](https://vinkius.com/ai-agent-connect/aws-cloudformation-stack-limits-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS CloudFormation Stack Limits Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-cloudformation-stack-limits-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS CloudFormation Stack Limits Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-cloudformation-stack-limits-calculator": {
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
