# AI Feature NPS Impact Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-nps-impact-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Quantify how AI features drive or drag your product's NPS.

## Description
This MCP server provides a specialized analytics engine to measure the specific impact of AI features on Net Promoter Score (NPS). By using tools like `calculate_nps_lift` and `evaluate_detractor_risk`, you can attribute sentiment shifts to AI usage, identify high-risk user segments, and translate satisfaction data into business value. It helps product teams understand if AI is a core driver of loyalty or a source of friction.


## Available Tools (4)
- **aggregate_segment_impact**: Provides a high-level summary of how AI is impacting different user demographics
- **calculate_nps_lift**: Determines how much the AI feature is driving or dragging the overall product NPS
- **evaluate_detractor_risk**: Predicts the likelihood of users becoming detractors based on their specific AI-related grievances
- **quantify_feature_value**: Translates NPS and satisfaction data into a business-centric Value Perception metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature NPS Impact Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NPS lift for an Enterprise user in a Data Analysis workflow where NPS with AI is 50 and without AI is 30."

**🤖 AI Agent:**
> The NPS lift is 20, and the AI feature is acting as a Driver for this segment.

---

**👤 You:**
> "What is the detractor risk for a daily user with an AI satisfaction score of 2 and reasons including 'hallucinations'?"

**🤖 AI Agent:**
> The risk level is Critical, with 'hallucinations' identified as the primary risk driver.

---

**👤 You:**
> "Determine the value perception for a feature with an NPS lift of 15 and AI satisfaction of 80 in a Content Creation use case."

**🤖 AI Agent:**
> The feature is categorized as an Essential core value driver.


## ❓ FAQ

**Q: How does the engine calculate NPS lift?**
The `calculate_nps_lift` tool calculates the absolute difference between the NPS of users interacting with the AI feature and the baseline NPS of users who do not.

**Q: Can I predict user churn using this tool?**
Yes, by using `evaluate_detractor_risk`, you can predict the likelihood of users becoming detractors based on their AI satisfaction and specific grievances.

**Q: What is the purpose of quantifying feature value?**
The `quantify_feature_value` tool translates NPS and satisfaction data into a business-centric metric that categorizes the feature as Essential, Nice-to-have, or a Commodity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-nps-impact-engine](https://vinkius.com/ai-agent-connect/ai-feature-nps-impact-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature NPS Impact Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-nps-impact-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature NPS Impact Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-nps-impact-engine": {
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
