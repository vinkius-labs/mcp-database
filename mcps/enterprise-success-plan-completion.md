# Enterprise Success Plan Completion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-success-plan-completion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enterprise](../categories/enterprise.md)

Calculates success plan achievement rates, outcome scores, and renewal predictability.

## Description
This MCP server provides advanced analytics for enterprise success plans. It allows AI agents to calculate the `get_plan_completion_status` to track milestone progress, `get_outcome_achievement_score` to measure realized business value, `get_ttv_efficiency_metric` to evaluate time-to-value efficiency, and `get_renewal_predictability_index` to assess customer renewal risk based on current health metrics.


## Available Tools (4)
- **get_outcome_achievement_score**: Calculates the achievement score based on reached outcomes and their importance
- **get_plan_completion_status**: Calculates the completion rate and weighted completion rate of milestones
- **get_renewal_predictability_index**: Predicts renewal probability and determines risk level
- **get_ttv_efficiency_metric**: Calculates the efficiency ratio of time to value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Success Plan Completion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current completion status of our success plan with these milestones: { "milestones": [{"completed": true, "relevanceWeight": 5}, {"completed": false, "relevanceWeight": 10}] }?"

**🤖 AI Agent:**
> The raw completion rate is 50%, and the weighted completion rate is 33.3%.

---

**👤 You:**
> "How much business value has been realized with these outcomes: { "outcomes": [{"reached": true, "importanceLevel": 8}, {"reached": false, "importanceLevel": 2}] }?"

**🤖 AI Agent:**
> The current outcome achievement score is 0.8.

---

**👤 You:**
> "Calculate the renewal probability for a customer with 0.8 completion, 0.7 outcome score, 0.5 TTV ratio, and 0.6 resource utilization."

**🤖 AI Agent:**
> The renewal probability is 85% with a Low risk level.


## ❓ FAQ

**Q: How is the completion rate calculated?**
The `get_plan_completion_status` tool calculates both a raw completion rate and a weighted completion rate based on the relevance of each milestone.

**Q: Can I predict if a customer will renew?**
Yes, using the `get_renewal_predictability_index` tool, you can determine the renewal probability and risk level by analyzing completion, outcomes, and efficiency.

**Q: What is Time to Value (TTV)?**
TTV is the duration until the first significant outcome is achieved. The `get_ttv_efficiency_metric` tool helps compare this against the planned duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-success-plan-completion](https://vinkius.com/ai-agent-connect/enterprise-success-plan-completion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Success Plan Completion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-success-plan-completion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Success Plan Completion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-success-plan-completion": {
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
