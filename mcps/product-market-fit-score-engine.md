# Product-Market Fit Score Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/product-market-fit-score-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Quantify product-market fit using Sean Ellis methodology and business metrics.

## Description
This MCP server provides a diagnostic engine to quantify Product-Market Fit (PMF). It synthesizes qualitative user sentiment from the Sean Ellis test with quantitative business health metrics like retention and organic growth. Use `calculate_sentiment_metrics` to analyze survey responses, `calculate_pmf_composite_score` to generate a 0-100 index, `analyze_cohort_variance` to adjust for early adopter bias, and `get_market_readiness_guidance` to receive actionable business directions.


## Available Tools (4)
- **get_market_readiness_guidance**: Translates the PMF score and readiness level into actionable business directions
- **calculate_sentiment_metrics**: Analyzes raw survey responses to determine the qualitative health of the product
- **analyze_cohort_variance**: Adjusts the PMF score to account for potential bias between early adopters and the broader market
- **calculate_pmf_composite_score**: Generates the final 0-100 PMF score by combining qualitative sentiment and quantitative business metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product-Market Fit Score Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these survey responses: ['very disappointed', 'somewhat disappointed', 'very disappointed', 'not disappointed']."

**🤖 AI Agent:**
> The very disappointed percentage is 50% with a total of 4 responses.

---

**👤 You:**
> "Calculate the PMF score with 40% very disappointed, 30 NPS, 45% retention, and 15% organic growth."

**🤖 AI Agent:**
> The calculated PMF score is 65, indicating an Optimization readiness level.

---

**👤 You:**
> "What is the recommended action for a PMF score of 85 and 20% retention?"

**🤖 AI Agent:**
> The primary focus should be on Product Stability due to the high score paired with low retention.


## ❓ FAQ

**Q: What is the Sean Ellis test?**
It is a qualitative survey method that asks users how they would feel if they could no longer use the product, identifying the 'very disappointed' segment.

**Q: How is the PMF score calculated?**
The score is a weighted composite index combining the 'very disappointed' percentage with NPS, retention rate, and organic growth.

**Q: Can I adjust for early adopter bias?**
Yes, use `analyze_cohort_variance` to adjust the score based on cohort age and sample size to account for potential over-reporting of satisfaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/product-market-fit-score-engine](https://vinkius.com/en/ai-agent-connect/product-market-fit-score-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product-Market Fit Score Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-market-fit-score-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product-Market Fit Score Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-market-fit-score-engine": {
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
