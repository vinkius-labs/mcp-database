# GuardDuty Findings Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/guardduty-findings-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Project AWS GuardDuty finding volumes, detection source requirements, and resource overhead.

## Description
This MCP server provides deterministic calculations for AWS GuardDuty operations. Use `calculate_finding_projections` to estimate daily finding volumes and severity distributions based on event throughput. Use `calculate_infrastructure_requirements` to determine the breakdown of detection sources like CloudTrail and VPC Flow Logs, as well as resource overhead for EKS and ECS Fargate runtime monitoring. Finally, use `calculate_governance_recommendations` to get administrative guidelines for suppression rules, archive periods, and the number of administrators required for your account scale.


## Available Tools (3)
- **calculate_finding_projections**: Estimates the total number of findings and their severity distribution based on event throughput
- **calculate_governance_recommendations**: Provides administrative guidelines for account management and finding lifecycle
- **calculate_infrastructure_requirements**: Determines the detection source breakdown and specific resource overhead for runtime monitoring


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GuardDuty Findings Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate findings for 5 accounts with 500 events per second and S3/EKS enabled."

**🤖 AI Agent:**
> The projected daily findings are 43,200, with a distribution of Info, Low, Medium, and High severities based on your enabled sources.

---

**👤 You:**
> "What are the infrastructure requirements for 10 EKS nodes with Runtime monitoring enabled?"

**🤖 AI Agent:**
> The EKS agent will require 1000 MB of total memory (100 MB per node) for runtime monitoring.

---

**👤 You:**
> "How many administrators do I need for 2500 AWS accounts?"

**🤖 AI Agent:**
> You will need 3 administrators to manage 2500 accounts based on the recommended threshold.


## ❓ FAQ

**Q: How do I estimate my daily finding volume?**
You can use the `calculate_finding_projections` tool. Provide the total number of AWS accounts and the estimated average number of raw log events processed per second.

**Q: Does runtime monitoring add resource overhead?**
Yes. For EKS, the `calculate_infrastructure_requirements` tool calculates a 100 MB memory overhead per node. For ECS Fargate, it flags the sidecar container overhead.

**Q: What are the recommended governance settings?**
The `calculate_governance_recommendations` tool suggests up to 100 suppression rules and a 90-day archive period based on your account count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/guardduty-findings-calculator](https://vinkius.com/ai-agent-connect/guardduty-findings-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GuardDuty Findings Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `guardduty-findings-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GuardDuty Findings Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guardduty-findings-calculator": {
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
