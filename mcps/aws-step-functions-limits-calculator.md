# AWS Step Functions Limits Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-step-functions-limits-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Validate AWS Step Functions configurations against hard service limits and performance best practices.

## Description
This MCP server provides deterministic tools to evaluate AWS Step Functions state machine configurations. It checks for hard service limits such as definition size and execution history capacity, while also providing performance recommendations for state counts and nesting depth. Use `check_definition_compliance` to verify if your JSON definition or event history exceeds AWS constraints, and `calculate_workflow_capacities` to determine payload and duration limits for Standard or Express workflows.


## Available Tools (4)
- **calculate_activity_timeout_range**: Determines the valid window for activity task timeouts
- **calculate_workflow_capacities**: Calculates the available or allowed capacities for data payloads, duration, and state naming based on the workflow mode
- **check_definition_compliance**: Validates if the provided state machine definition and structure exceed hard AWS service limits
- **evaluate_performance_recommendations**: Compares the current configuration against AWS best practices and soft limits to prevent performance degradation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Step Functions Limits Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my state machine definition compliant if it is 120 KB?"

**🤖 AI Agent:**
> No, a 120 KB definition exceeds the hard limit of 104,857 characters.

---

**👤 You:**
> "What are the payload limits for an Express workflow?"

**🤖 AI Agent:**
> The maximum payload size for an Express workflow is 32 KB.

---

**👤 You:**
> "What is the recommended maximum number of states?"

**🤖 AI Agent:**
> It is recommended to keep the state count at or below 200 for optimal performance.


## ❓ FAQ

**Q: How do I check if my state machine definition is too large?**
You can use the `check_definition_compliance` tool by providing your definition size in KB to identify if it exceeds the 104,857 character limit.

**Q: What is the difference between Standard and Express workflow limits?**
Standard workflows allow up to 256 KB payloads and 1 year duration, while Express workflows are limited to 32 KB payloads and 5 minutes duration. Use `calculate_workflow_capacities` to see the exact values.

**Q: Can I check for performance bottlenecks?**
Yes, the `evaluate_performance_recommendations` tool checks if your state count or nesting depth exceeds AWS best practices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-step-functions-limits-calculator](https://vinkius.com/ai-agent-connect/aws-step-functions-limits-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Step Functions Limits Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-step-functions-limits-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Step Functions Limits Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-step-functions-limits-calculator": {
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
