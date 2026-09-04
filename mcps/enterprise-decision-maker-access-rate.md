# Enterprise Decision Maker Access Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-decision-maker-access-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Quantify sales engagement effectiveness and decision maker access success.

## Description
This MCP server provides specialized analytics to measure how effectively sales teams reach key organizational stakeholders. By analyzing engagement data, it calculates the `access_rate` of decision makers, evaluates the resistance caused by gatekeepers using `evaluate_gatekeeper_friction`, and determines if reaching decision makers correlates with winning deals via `analyze_win_correlation`. It also provides actionable guidance through `recommend_access_strategy` to optimize outreach based on current performance metrics.


## Available Tools (4)
- **analyze_win_correlation**: Analyzes the statistical link between DM engagement and deal wins
- **calculate_access_metrics**: Calculates efficiency metrics for reaching decision makers
- **evaluate_gatekeeper_friction**: Evaluates the resistance encountered due to organizational layers
- **recommend_access_strategy**: Recommends a strategic approach based on performance metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Decision Maker Access Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current efficiency in reaching decision makers with 50 DMs in pipeline, 10 engaged, and 40 attempts?"

**🤖 AI Agent:**
> Your current access rate is 20%, with an engagement efficiency of 0.25 and an attempt intensity of 4.0.

---

**👤 You:**
> "Does reaching decision makers actually lead to winning more deals based on this data: 5 engaged, 4 won, 1 lost?"

**🤖 AI Agent:**
> There is a high correlation between decision maker engagement and deal wins, indicating that reaching these stakeholders is a critical driver of revenue.

---

**👤 You:**
> "How much friction are we facing with 100 attempts, 20 non-DM interactions, and 30 DM interactions?"

**🤖 AI Agent:**
> The friction index is high, suggesting a deep or complex organizational structure that requires more effort to penetrate.


## ❓ FAQ

**Q: How is the access rate calculated?**
The access rate is the percentage of total decision makers in your pipeline who have been successfully engaged through meaningful interactions.

**Q: Can I identify if gatekeepers are blocking my progress?**
Yes, you can use the `evaluate_gatekeeper_friction` tool to measure the resistance encountered from non-decision-making stakeholders.

**Q: How do I get advice on improving my sales outreach?**
You can use the `recommend_access_strategy` tool, which provides tactical adjustments and strategic directions based on your current access rate and friction levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-decision-maker-access-rate](https://vinkius.com/ai-agent-connect/enterprise-decision-maker-access-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Decision Maker Access Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-decision-maker-access-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Decision Maker Access Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-decision-maker-access-rate": {
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
