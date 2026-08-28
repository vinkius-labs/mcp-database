# AI Suggestion Effectiveness Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-suggestion-effectiveness-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze AI suggestion acceptance, modification, and quality metrics.

## Description
This MCP server provides tools to evaluate the effectiveness of AI-driven suggestions in SaaS environments. It calculates key performance indicators including acceptance rates, modification rates, and a composite quality score. Use `get_suggestion_acceptance_metrics` to get raw performance data, `get_quality_score_report` to determine overall value, `get_type_performance_breakdown` to identify high-performing suggestion categories, and `get_contextual_efficiency_rating` to assess if suggestion timing is optimal.


## Available Tools (4)
- **get_contextual_efficiency_rating**: Evaluates the efficiency of suggestion timing relative to user action
- **get_quality_score_report**: Calculates the overall quality score and status of AI suggestions
- **get_suggestion_acceptance_metrics**: Calculates raw performance metrics for AI suggestions
- **get_type_performance_breakdown**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Suggestion Effectiveness Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the raw performance of my AI suggestions if 100 were shown, 40 were accepted, and 20 were modified?"

**🤖 AI Agent:**
> The acceptance rate is 40%, the modification rate is 20%, and the total interaction rate is 60%.

---

**👤 You:**
> "How is the quality score for these metrics: acceptance rate 0.5, modification rate 0.2, and they were proactive?"

**🤖 AI Agent:**
> The quality score is 0.85 and the status is Excellent.

---

**👤 You:**
> "Is the timing of a suggestion efficient if it appeared 2 seconds after an action and was accepted?"

**🤖 AI Agent:**
> The efficiency rating is 0.95.


## ❓ FAQ

**Q: How is the quality score calculated?**
The quality score combines acceptance and modification rates, giving higher weight to unmodified acceptances. It can also be adjusted based on whether suggestions were proactive.

**Q: Can I see which suggestion types are most effective?**
Yes, you can use `get_type_performance_breakdown` to see the specific acceptance rates for each category of suggestion.

**Q: What does the efficiency rating measure?**
The efficiency rating measures how well the timing of a suggestion aligns with user actions using `get_contextual_efficiency_rating`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-suggestion-effectiveness-analyzer](https://vinkius.com/ai-agent-connect/ai-suggestion-effectiveness-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Suggestion Effectiveness Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-suggestion-effectiveness-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Suggestion Effectiveness Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-suggestion-effectiveness-analyzer": {
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
