# AWS Disaster Recovery Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-disaster-recovery-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic RTO and RPO estimation for AWS disaster recovery strategies.

## Description
This MCP server provides precise calculations for disaster recovery planning on AWS. It allows AI agents to estimate Recovery Time Objective (RTO) and Recovery Point Objective (RPO) based on specific infrastructure parameters like RDS snapshot frequency, S3 replication latency, and Route 53 TTL. Use `calculate_dr_metrics` to determine cost ratios and testing frequencies, or `compare_rto_rpo_to_sla` to verify if your technical setup meets business requirements. It covers all major AWS DR patterns including backup-and-restore, pilot-light, warm-standby, and multi-site.


## Available Tools (3)
- **calculate_dr_metrics**: Calculates the RPO, RTO, cost ratio, and testing frequency for a selected disaster recovery strategy
- **validate_strategy_compatibility**: Checks if the provided technical parameters are logically compatible with the chosen DR strategy
- **compare_rto_rpo_to_sla**: Compares calculated metrics against a provided Service Level Agreement (SLA)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Disaster Recovery Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate DR metrics for a pilot-light strategy with 4 hour RDS snapshots, 15 minute S3 latency, 60 second Route 53 TTL, and 10 minute ASG warmup."

**🤖 AI Agent:**
> For a pilot-light strategy, the RPO is 15 minutes and the RTO is 25 minutes. The estimated cost ratio is 0.2, and the recommended testing frequency is monthly.

---

**👤 You:**
> "What is the RPO and RTO for a multi-site AWS setup?"

**🤖 AI Agent:**
> For a multi-site strategy, the RPO is 0 minutes and the RTO is effectively 0 seconds.

---

**👤 You:**
> "Check if an RPO of 30 minutes and RTO of 60 minutes complies with an SLA of 45 minutes RPO and 120 minutes RTO."

**🤖 AI Agent:**
> The status is Compliant.


## ❓ FAQ

**Q: How is RPO calculated?**
RPO is determined by the maximum of the RDS snapshot frequency and the S3 cross-region replication latency. For multi-site strategies, RPO is zero.

**Q: Can I check if my DR strategy meets my business SLA?**
Yes, you can use the `compare_rto_rpo_to_sla` tool to compare your calculated metrics against your specific business requirements.

**Q: What DR strategies are supported?**
The server supports backup-and-restore, pilot-light, warm-standby, and multi-site strategies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-disaster-recovery-calculator](https://vinkius.com/ai-agent-connect/aws-disaster-recovery-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Disaster Recovery Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-disaster-recovery-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Disaster Recovery Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-disaster-recovery-calculator": {
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
