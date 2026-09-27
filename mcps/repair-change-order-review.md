# Repair Change Order Review MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-change-order-review)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Automated decision support for evaluating construction change orders.

## Description
This MCP server provides specialized tools for construction and infrastructure project managers to evaluate proposed changes to project scope. It uses a strict change-control rule to validate scope, price, schedule, and approval evidence. Use `analyze_change_order` to get a recommendation, `calculate_baseline_impact` to update project targets, `validate_alternatives` to check efficiency, and `audit_approval_chain` to verify authorization levels.


## Available Tools (4)
- **analyze_change_order**: Evaluates a proposed change against mandatory change-control rules
- **audit_approval_chain**: Verifies if the approval evidence matches the required authority levels
- **calculate_baseline_impact**: Determines the new project schedule and budget targets based on a successful change
- **validate_alternatives**: Assesses whether the proposed change is the most efficient path


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Change Order Review** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this change: Original scope was building a 50m wall. Proposed change is a 60m wall. Cost impact is $5000, schedule impact is 2 days. Reason is soil instability. Approval is from the Site Manager."

**🤖 AI Agent:**
> recommendation: approve, updatedBaseline: { newTotalBudget: [current + 5000], newTotalSchedule: [current + 2] }

---

**👤 You:**
> "The project needs an extra $50,000 for structural reinforcement. The schedule will slip by 10 days. The reason is unexpected foundation issues. We have approval from the Project Manager."

**🤖 AI Agent:**
> recommendation: defer, revisionQuestions: ["High-cost changes require Director or Executive level approval evidence."]

---

**👤 You:**
> "We are proposing a change to use steel instead of wood. The cost is $2000 more. We considered using composite but it was too expensive. The original scope was timber framing."

**🤖 AI Agent:**
> recommendation: negotiate, revisionQuestions: ["Please provide more detail on why the composite alternative was rejected."]


## ❓ FAQ

**Q: How does the tool decide to approve a change?**
The `analyze_change_order` tool requires all mandatory fields including scope, cost, schedule, and `approvalEvidence` to be present to consider an approval.

**Q: Can I update my project budget after a change is approved?**
Yes, once a change is validated, you can use `calculate_baseline_impact` to determine the new total budget and schedule.

**Q: What happens if the approval evidence is insufficient?**
If the `audit_approval_chain` tool finds that the evidence does not match the required authority level for the cost impact, the recommendation will be to defer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-change-order-review](https://vinkius.com/en/ai-agent-connect/repair-change-order-review)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Change Order Review** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-change-order-review` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Change Order Review** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-change-order-review": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
