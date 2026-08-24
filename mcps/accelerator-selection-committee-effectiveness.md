# Accelerator Selection Committee Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-selection-committee-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Evaluate the reliability, predictive accuracy, and decision-making quality of selection committees.

## Description
This MCP server provides diagnostic tools to analyze how effectively a committee selects high-potential candidates. It measures the tension between speed, consensus, and predictive accuracy to ensure decision-making rigor. Use `get_committee_reliability` to assess stability, `get_predictive_performance` to evaluate selection success, and `get_calibration_requirements` to identify necessary strategic adjustments like increasing diversity or standardizing criteria.


## Available Tools (3)
- **get_calibration_requirements**: Identify if the committee needs to adjust its selection thresholds or diversity levels
- **get_committee_reliability**: Determine the overall consistency and stability of the committee's decision-making process
- **get_predictive_performance**: Assess how well the committee's selections align with real-world or projected success


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Selection Committee Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How stable is our selection committee with 10 members, a 5% reversal rate, and 85% agreement?"

**🤖 AI Agent:**
> The committee is Stable with a reliability score of 82.5 and a high consensus level.

---

**👤 You:**
> "Evaluate the performance of a committee that made 50 decisions with 90% accuracy in an average of 2 days."

**🤖 AI Agent:**
> The committee has an accuracy score of 0.9 and an efficient rating.

---

**👤 You:**
> "What adjustments are needed if agreement is 95% but accuracy is only 60% with a diversity score of 40?"

**🤖 AI Agent:**
> The recommended action is to Increase Diversity to mitigate the risk of groupthink.


## ❓ FAQ

**Q: How is committee reliability calculated?**
Reliability is determined using `get_committee_reliability`, which analyzes the number of committee members, the reversal rate of decisions, and the level of inter-rater agreement.

**Q: Can this tool help prevent groupthink?**
Yes. By using `get_calibration_requirements`, the tool can identify if high agreement coupled with low accuracy indicates a need to increase diversity to combat groupthink.

**Q: What metrics are used for predictive performance?**
The `get_predictive_performance` tool evaluates decisions made, prediction accuracy, and decision speed to provide an efficiency rating and performance profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-selection-committee-effectiveness](https://vinkius.com/ai-agent-connect/accelerator-selection-committee-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Selection Committee Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-selection-committee-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Selection Committee Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-selection-committee-effectiveness": {
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
