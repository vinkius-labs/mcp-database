# Enterprise Discovery Call Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-discovery-call-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-analytics](../categories/sales-analytics.md)

Quantify the quality and outcome potential of enterprise sales discovery calls.

## Description
This MCP server provides an analytics engine to evaluate enterprise sales discovery calls. It quantifies call quality by analyzing question depth, pain point identification, stakeholder coverage, and momentum. Use `calculate_call_score` to get a weighted performance rating, `evaluate_information_depth` to check proposal readiness, `assess_stakeholder_coverage` to identify engagement risks, and `analyze_followup_momentum` to measure deal velocity.


## Available Tools (4)
- **assess_stakeholder_coverage**: Analyze if the correct organizational breadth was achieved during the call
- **calculate_call_score**: Provide a comprehensive performance rating for a specific discovery call
- **evaluate_information_depth**: Determine if the information gathered is sufficient to move to a proposal stage
- **analyze_followup_momentum**: Evaluate if the call resulted in actionable next steps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Discovery Call Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for call ID 'call_123' where 8 questions were answered, 3 pain points were identified, 4 stakeholders were mapped, and it is a high complexity deal."

**🤖 AI Agent:**
> The discovery score for call 'call_123' is 85. The completeness is 85%, momentum is High, and the risk assessment is Low due to sufficient stakeholder mapping.

---

**👤 You:**
> "Is this call ready for a proposal? I answered 5 questions and identified 1 pain point for a medium complexity deal."

**🤖 AI Agent:**
> No, the deal is not ready for a proposal. The depth score is low because the number of confirmed pain points is insufficient for a medium complexity deal.

---

**👤 You:**
> "Check the momentum for a call where next steps were agreed and we confirmed access to a new stakeholder in a high complexity deal."

**🤖 AI Agent:**
> The momentum score is 95. The follow-up quality is Exceptional, and the next step clarity is high because a new stakeholder was successfully engaged.


## ❓ FAQ

**Q: How is the discovery score calculated?**
The score is a weighted aggregation of answered questions, confirmed pain points, and stakeholder mapping, adjusted by the deal's complexity level.

**Q: Can I use this to identify single-threaded deal risks?**
Yes, by using `assess_stakeholder_coverage`, you can identify engagement risks and determine if you have sufficient organizational breadth to avoid single-threaded deals.

**Q: What determines if a deal is ready for a proposal?**
The `evaluate_information_depth` tool determines readiness based on the ratio of pain points identified to questions answered, relative to the deal complexity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-discovery-call-effectiveness](https://vinkius.com/ai-agent-connect/enterprise-discovery-call-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Discovery Call Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-discovery-call-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Discovery Call Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-discovery-call-effectiveness": {
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
