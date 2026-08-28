# AI Feature Expansion Impact Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-expansion-impact-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the financial and behavioral impact of AI features on SaaS expansion revenue and upsell conversion.

## Description
This MCP server provides a suite of analytical tools to measure how AI capabilities drive growth in SaaS businesses. By analyzing revenue cohorts and user behavior, you can determine the exact expansion lift provided by AI features. Use `calculate_expansion_lift` to compare revenue growth between AI and non-AI users, `analyze_upsell_conversion` to track tier upgrades, and `attribute_ai_revenue` to distribute expansion revenue to specific features based on usage intensity and value perception. It is designed to help product and finance teams understand the true ROI of AI investments.


## Available Tools (4)
- **analyze_upsell_conversion**: Measures how effectively AI features drive users to upgrade their subscription tiers
- **attribute_ai_revenue**: Distributes expansion revenue to specific AI features based on usage patterns and perceived value
- **calculate_expansion_lift**: Determines the relative revenue growth boost provided by AI features
- **evaluate_feature_impact_summary**: Provides a high-level health check of AI feature contribution across the entire customer base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature Expansion Impact Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expansion lift if AI users generated $50,000 and non-AI users generated $30,000?"

**🤖 AI Agent:**
> The expansion lift is 66.67%.

---

**👤 You:**
> "Compare upsell rates: 100 AI users with 20 upgrades vs 100 non-AI users with 5 upgrades."

**🤖 AI Agent:**
> The AI conversion rate is 20%, the non-AI conversion rate is 5%, resulting in a conversion delta of 15%.

---

**👤 You:**
> "Give me a summary of AI contribution if AI revenue is $10,000, non-AI revenue is $10,000, AI users are 50, and non-AI users are 50."

**🤖 AI Agent:**
> The AI revenue contribution is 50% and the AI user density is 50%.


## ❓ FAQ

**Q: How do I calculate the revenue boost from AI features?**
You can use the `calculate_expansion_lift` tool. Provide the total expansion revenue from users who use AI and the revenue from those who do not.

**Q: Can I attribute revenue to specific AI tools?**
Yes, the `attribute_ai_revenue` tool allows you to distribute expansion revenue to specific features using usage metrics and value perception scores.

**Q: How does this help with subscription upgrades?**
The `analyze_upsell_conversion` tool measures the conversion rate of AI users compared to non-AI users to see if AI adoption drives tier upgrades.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-expansion-impact-analyzer](https://vinkius.com/ai-agent-connect/ai-feature-expansion-impact-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature Expansion Impact Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-expansion-impact-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature Expansion Impact Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-expansion-impact-analyzer": {
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
