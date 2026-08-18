# AWS Well-Architected Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-well-architected-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

A deterministic engine for evaluating AWS infrastructure against the six Well-Architected Framework pillars.

## Description
This MCP server provides a precise scoring engine to evaluate AWS workloads against the six foundational pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability. Use `calculate_pillar_metrics` to assess individual pillar health, `generate_improvement_plan` to create prioritized remediation roadmaps, `evaluate_workload_alignment` for specialized lens analysis (SaaS, HPC, IoT), and `track_risk_trend` to monitor risk changes over time.


## Available Tools (4)
- **calculate_pillar_metrics**: Evaluates the health and risk density of an individual architectural pillar
- **evaluate_workload_alignment**: Calculates how well the workload adheres to specific architectural patterns and lenses
- **generate_improvement_plan**: Produces a prioritized roadmap for remediating architectural weaknesses
- **track_risk_trend**: Analyzes changes in risk profile over multiple assessment periods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Well-Architected Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for the Security pillar with these responses: [{"riskLevel": "None"}, {"riskLevel": "High"}, {"riskLevel": "Medium"}]"

**🤖 AI Agent:**
> {"pillarScore": 66.67, "highRiskCount": 1, "status": "Healthy"}

---

**👤 You:**
> "What is the trend if my current score is 85 and my previous scores were [70, 75, 80]?"

**🤖 AI Agent:**
> {"trendStatus": "improving", "delta": 5}

---

**👤 You:**
> "Generate an improvement plan for these pillar results: [{"pillarName": "Security", "pillarScore": 40, "highRiskCount": 6}] and these high risk details: [{"pillarName": "Security", "description": "Unencrypted S3 buckets"}]"

**🤖 AI Agent:**
> {"prioritizedTasks": ["Remediate Unencrypted S3 buckets"], "milestoneCount": 1}


## ❓ FAQ

**Q: How is the pillar score calculated?**
The pillar score is the percentage of questions within that pillar that do not have a High risk level.

**Q: What is a 'Critical' status?**
A pillar is flagged as Critical if its score is below 50 or if it contains more than 5 High risk issues.

**Q: Can I use specialized lenses like SaaS or IoT?**
Yes, you can use `evaluate_workload_alignment` with specific lens types like SaaS, HPC, or IoT to get specialized scoring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-well-architected-score-calculator](https://vinkius.com/ai-agent-connect/aws-well-architected-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Well-Architected Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-well-architected-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Well-Architected Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-well-architected-score-calculator": {
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
