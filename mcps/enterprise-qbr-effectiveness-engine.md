# Enterprise QBR Effectiveness Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-qbr-effectiveness-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Quantify the business impact and operational quality of Quarterly Business Reviews.

## Description
This MCP server provides a strategic analytical engine to measure the success of Quarterly Business Reviews (QBRs). It allows AI agents to calculate effectiveness scores, evaluate stakeholder engagement levels, and quantify the financial ROI of strategic reviews. By using tools like `calculate_qbr_score`, `evaluate_stakeholder_engagement`, `get_qbr_roi`, and `query_qbr_trends`, agents can transform raw QBR data into actionable business intelligence regarding expansion opportunities and renewal correlations.


## Available Tools (4)
- **calculate_qbr_score**: Calculates the core effectiveness score for a specific QBR instance
- **evaluate_stakeholder_engagement**: Determines the qualitative engagement level of the client stakeholders
- **get_qbr_roi**: Quantifies the financial impact of the QBR activities
- **query_qbr_trends**: Analyzes historical effectiveness and engagement across a specific account or cohort


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise QBR Effectiveness Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the effectiveness score for QBR ID 12345 with 10 action items and 8 completed, plus a $50,000 expansion opportunity?"

**🤖 AI Agent:**
> The effectiveness score for QBR 12345 is 85, reflecting high action item completion and significant expansion value.

---

**👤 You:**
> "Calculate the ROI for QBR 9876 where we had $100,000 in expansion, a $500,000 renewal, and the QBR cost $5,000."

**🤖 AI Agent:**
> The total ROI for this QBR is $595,000, representing a highly profitable strategic review.

---

**👤 You:**
> "Evaluate the engagement for QBR 555 where the attendees were CEO, Manager, and User, with executive presence and 90% follow-through."

**🤖 AI Agent:**
> The engagement level is High, as the CEO was present and the client demonstrated strong follow-through.


## ❓ FAQ

**Q: How is the QBR effectiveness score calculated?**
The score is determined using `calculate_qbr_score`, which evaluates the completion rate of action items and the presence of expansion opportunities.

**Q: Can I track engagement trends over time?**
Yes, you can use `query_qbr_trends` to analyze historical effectiveness and engagement levels for a specific account over a defined timeframe.

**Q: How does the tool calculate ROI?**
The `get_qbr_roi` tool aggregates renewal values and expansion opportunities, then subtracts the operational cost of the QBR to find the net value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-qbr-effectiveness-engine](https://vinkius.com/ai-agent-connect/enterprise-qbr-effectiveness-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise QBR Effectiveness Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-qbr-effectiveness-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise QBR Effectiveness Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-qbr-effectiveness-engine": {
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
