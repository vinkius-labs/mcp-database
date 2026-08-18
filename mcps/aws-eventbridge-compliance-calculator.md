# AWS EventBridge Compliance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-eventbridge-compliance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Deterministic tool for calculating AWS EventBridge architectural compliance and resource limits.

## Description
This MCP server provides a deterministic way to validate AWS EventBridge architectures. It checks event payloads against the 256 KB limit, evaluates pattern nesting depth, and calculates routing capacity for rules and targets. Use `calculate_event_compliance` to verify payload and nesting, `calculate_routing_capacity` to check bus and rule limits, and `calculate_governance_and_resiliency` to ensure your storage, schema, and retry policies align with AWS best practices.


## Available Tools (3)
- **calculate_governance_and_resiliency**: Checks the configuration against recommended best practices for storage, schema management, and error handling
- **calculate_event_compliance**: Determines if a specific event configuration adheres to hard AWS service limits
- **calculate_routing_capacity**: Evaluates the capacity of event buses and the routing capabilities of rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS EventBridge Compliance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my event configuration valid for a 300 KB payload and 6 levels of nesting?"

**🤖 AI Agent:**
> No, the configuration is invalid. The event size exceeds the 256 KB limit and the nesting depth exceeds the maximum of 5 levels.

---

**👤 You:**
> "Check if 250 rules with 4 targets each is a valid routing configuration."

**🤖 AI Agent:**
> Yes, the configuration is valid. 250 rules is within the 300 rule limit, and 4 targets per rule is within the 5 target limit.

---

**👤 You:**
> "Validate a setup with 15 archives and 200 schema versions."

**🤖 AI Agent:**
> The configuration exceeds recommended best practices. It is recommended to stay within 10 archives and 100 schema versions.


## ❓ FAQ

**Q: What is the maximum event size supported?**
AWS EventBridge has a hard limit of 256 KB per event payload. The `calculate_event_compliance` tool can verify if your event size is within this limit.

**Q: How many rules can I have per event bus?**
A single event bus can support up to 300 rules. You can use `calculate_routing_capacity` to check if your rule count is compliant.

**Q: Can I check my retry policy compliance?**
Yes, the `calculate_governance_and_resiliency` tool validates that your retry count does not exceed 185 attempts and stays within a 24-hour window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-eventbridge-compliance-calculator](https://vinkius.com/ai-agent-connect/aws-eventbridge-compliance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS EventBridge Compliance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-eventbridge-compliance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS EventBridge Compliance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-eventbridge-compliance-calculator": {
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
