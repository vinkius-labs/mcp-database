# Enterprise Qualification Framework MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-qualification-framework)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify sales opportunity health using BANT and MEDDIC methodologies.

## Description
This MCP server provides decision-support tools to quantify the health of enterprise sales opportunities. By applying BANT (Budget, Authority, Need, Timeline) and MEDDIC principles, it identifies gaps in the sales cycle and detects disqualification risks. Use `calculate_qualification_score` to get a numerical health rating, `perform_gap_analysis` to find missing qualification dimensions, `check_disqualification_triggers` to identify deals that should be removed from the pipeline, and `evaluate_competition_impact` to assess competitive risks.


## Available Tools (4)
- **calculate_qualification_score**: Provides a single numerical health rating and a summary of the opportunity's viability
- **check_disqualification_triggers**: Performs a high-speed check to see if the deal should be immediately removed from the pipeline
- **evaluate_competition_impact**: Analyzes how the current competitive landscape affects the probability of winning
- **perform_gap_analysis**: Identifies specifically which qualification dimensions are missing or weak


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Qualification Framework** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the health score for a deal where budget is confirmed, authority is identified, need is validated, and timeline is established, but there is multi-vendor competition and no champion?"

**🤖 AI Agent:**
> The qualification score is 65. The opportunity is at medium risk due to multi-vendor competition and the absence of a confirmed champion.

---

**👤 You:**
> "Check if this deal should be disqualified: budget is not confirmed, but authority and need are validated."

**🤖 AI Agent:**
> The deal is disqualified. Reason: Budget has not been confirmed.

---

**👤 You:**
> "Perform a gap analysis for an opportunity with confirmed budget, identified authority, and a validated need, but no timeline or champion."

**🤖 AI Agent:**
> Missing dimensions: Timeline, Champion. Risk level: Medium. Recommendation: Establish a decision timeline and identify an internal advocate to increase win probability.


## ❓ FAQ

**Q: How is the qualification score calculated?**
The score is a weighted aggregate of BANT components. The presence of a Champion provides a significant boost, while high competition reduces the score unless authority and a champion are confirmed.

**Q: What triggers an automatic disqualification?**
A deal is automatically disqualified if any core BANT elements--Budget, Authority, or Need--are not confirmed.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-qualification-framework](https://vinkius.com/ai-agent-connect/enterprise-qualification-framework)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Qualification Framework** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-qualification-framework` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Qualification Framework** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-qualification-framework": {
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
