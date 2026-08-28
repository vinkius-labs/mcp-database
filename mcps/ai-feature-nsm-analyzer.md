# AI Feature NSM Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-nsm-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Calculates AI feature impact on North Star Metrics using correlation and leading indicators.

## Description
This MCP server provides a mathematical framework to measure how AI-driven features drive a company's North Star Metric (NSM). By analyzing the relationship between feature usage and core product goals, it enables data-driven product decisions. Use `get_nsm_contribution` to find the percentage of metric movement attributed to a feature, `evaluate_leading_indicator` to assess predictive signals, and `rank_feature_priority` to balance mathematical impact with strategic alignment. It helps product teams move from intuition to precise impact measurement.


## Available Tools (4)
- **evaluate_leading_indicator**: Determines how predictive a specific leading indicator is for the North Star Metric
- **get_feature_impact_summary**: Provides a high-level overview of a feature's health and contribution status
- **get_nsm_contribution**: Calculates the specific percentage of the North Star Metric that is driven by a specific AI feature
- **rank_feature_priority**: Generates a final priority ranking for an AI feature by combining mathematical impact with strategic intent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature NSM Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the contribution of our new autocomplete feature to our Daily Active Users NSM?"

**🤖 AI Agent:**
> The autocomplete feature contributes 4.5% to the Daily Active Users NSM, with a medium impact magnitude.

---

**👤 You:**
> "How reliable is the 'AI prompt completion' metric as a signal for our North Star Metric?"

**🤖 AI Agent:**
> The 'AI prompt completion' metric has a predictive strength of 0.85 and is considered a Stable signal.

---

**👤 You:**
> "Should we prioritize the 'Smart Summary' feature over 'Voice Input'?"

**🤖 AI Agent:**
> Based on the current metrics, 'Smart Summary' is ranked as P0 - Immediate due to its high NSM contribution and strategic alignment, while 'Voice Input' is ranked as P2 - Backlog.


## ❓ FAQ

**Q: How is the AI contribution calculated?**
The contribution is determined by the product of the feature usage volume and its correlation strength, normalized against the total NSM value using the `get_nsm_contribution` tool.

**Q: Can I use this to prioritize my product roadmap?**
Yes. By using `rank_feature_priority`, you can combine NSM contribution, indicator strength, and strategic alignment to generate a prioritized list of AI features.

**Q: What are leading indicators in this context?**
Leading indicators are predictive metrics that move before the NSM. You can use `evaluate_leading_indicator` to determine how reliably these signals predict future North Star Metric changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-nsm-analyzer](https://vinkius.com/ai-agent-connect/ai-feature-nsm-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature NSM Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-nsm-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature NSM Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-nsm-analyzer": {
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
