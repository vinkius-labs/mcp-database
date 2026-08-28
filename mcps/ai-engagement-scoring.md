# AI Engagement Scoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-engagement-scoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze AI feature engagement, adoption rates, and churn risk.

## Description
This MCP server provides deep insights into how users interact with AI capabilities. It allows agents to calculate a holistic engagement score, track feature adoption through discovery and realization rates, monitor engagement trends, and predict churn risk. By using tools like `calculate_user_engagement_score` and `predict_user_churn_risk`, agents can distinguish between simple feature testing and true value realization in AI workflows.


## Available Tools (4)
- **analyze_engagement_trend**: Track the trajectory of a user's interest in AI features over time
- **calculate_user_engagement_score**: Determine the current engagement level of a specific user
- **get_feature_adoption_metrics**: Evaluate how well specific AI features are being discovered and adopted
- **predict_user_churn_risk**: Identify users at risk of abandoning AI features


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Engagement Scoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current engagement score for user_123?"

**🤖 AI Agent:**
> The current engagement score for user_123 is 85, indicating a Power User with high value realization.

---

**👤 You:**
> "Is user_456 at risk of churning from our AI features?"

**🤖 AI Agent:**
> User_456 is flagged with a high risk level due to a declining engagement trend and low recent value realization.

---

**👤 You:**
> "How is the 'smart_summary' feature performing in terms of adoption?"

**🤖 AI Agent:**
> The 'smart_summary' feature has a high discovery rate of 75% but a lower realization rate of 30%, suggesting users are trying it but not finding consistent value.


## ❓ FAQ

**Q: How is the engagement score calculated?**
The score is determined by `calculate_user_engagement_score`, which evaluates session volume, feature breadth, and the ratio of successful value realizations to total AI outputs.

**Q: Can I predict which users might stop using AI features?**
Yes, you can use `predict_user_churn_risk` to identify users showing declining engagement trends and low value realization.

**Q: How do I measure if a new AI feature is successful?**
Use `get_feature_adoption_metrics` to compare the discovery rate against the realization rate, which measures how many users actually find value in the feature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-engagement-scoring](https://vinkius.com/ai-agent-connect/ai-engagement-scoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Engagement Scoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-engagement-scoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Engagement Scoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-engagement-scoring": {
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
