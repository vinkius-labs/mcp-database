# AWS Config Coverage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-config-coverage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate AWS Config rule limits, resource coverage, and infrastructure requirements.

## Description
This MCP server provides deterministic calculations for AWS Config deployments. Use `get_rule_limits` to verify if your rule count fits within standard (150) or increased (3000) limits. Use `get_resource_coverage` to check if your resource count per account stays within the recommended 100,000 threshold. Plan your deployment architecture with `get_infrastructure_plan` to determine the necessary recorders and delivery channels, or use `get_compliance_summary` to evaluate conformance packs and remediation actions.


## Available Tools (4)
- **get_rule_limits**: Determines if the requested number of Config rules is within standard or increased limits
- **get_compliance_summary**: Provides an overview of conformance packs, remediation actions, and snapshots based on the scale of the deployment
- **get_infrastructure_plan**: Calculates the required service components (Recorders, Channels, Aggregators) based on the account and regional footprint
- **get_resource_coverage**: Evaluates if the resource count per account is within the recommended operational threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Config Coverage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I deploy 200 Config rules in my account?"

**🤖 AI Agent:**
> Yes, 200 rules is within the increased limit of 3,000 rules per account.

---

**👤 You:**
> "What happens if I have 150,000 resources in one account?"

**🤖 AI Agent:**
> Your resource count exceeds the recommended threshold of 100,000 resources per account.

---

**👤 You:**
> "How many recorders do I need for 5 accounts across 3 regions?"

**🤖 AI Agent:**
> You will need 15 recorders in total, as each account requires one recorder per enabled region.


## ❓ FAQ

**Q: What is the standard limit for AWS Config rules?**
The standard limit is 150 rules per account, though this can be increased up to 3,000.

**Q: How many resources are recommended per AWS account?**
While there is no hard limit, it is recommended to maintain 100,000 resources or fewer per account for optimal performance.

**Q: How do I calculate the number of recorders needed?**
You can use the `get_infrastructure_plan` tool to calculate the total number of recorders based on your account and region count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-config-coverage-calculator](https://vinkius.com/ai-agent-connect/aws-config-coverage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Config Coverage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-config-coverage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Config Coverage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-config-coverage-calculator": {
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
