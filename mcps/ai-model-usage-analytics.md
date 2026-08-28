# AI Model Usage Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-model-usage-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze AI model cost distribution and usage concentration across product features.

## Description
This MCP server provides deep visibility into how AI model resources are consumed across your product. It allows you to calculate exact cost attribution per feature using `get_feature_cost_breakdown`, identify high-consumption areas with `analyze_usage_concentration`, and find cost-saving opportunities via `identify_optimization_targets`. You can also evaluate model selection effectiveness using `get_routing_efficiency_score` to ensure the most efficient models are being used for specific tasks.


## Available Tools (4)
- **get_feature_cost_breakdown**: To determine the exact monetary expenditure for each individual product feature
- **get_routing_efficiency_score**: To evaluate how effectively the system is selecting models for specific feature tasks
- **identify_optimization_targets**: To find features where costs are high but user engagement is low, or where model selection appears inefficient
- **analyze_usage_concentration**: To identify which features are the primary drivers of AI model consumption


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Model Usage Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the cost breakdown for features 'chat-v1' and 'image-gen-v2'."

**🤖 AI Agent:**
> The cost breakdown is: 'chat-v1' has a total cost of $450.00 with 1,200 calls, and 'image-gen-v2' has a total cost of $1,200.00 with 300 calls.

---

**👤 You:**
> "Which features are consuming the most AI resources?"

**🤖 AI Agent:**
> The primary drivers of consumption are 'summarizer-pro' (65% of total calls) and 'translator-api' (20% of total calls).

---

**👤 You:**
> "Are there any optimization opportunities for my features?"

**🤖 AI Agent:**
> Yes, 'legacy-parser' is a high-cost feature with low engagement, offering a potential savings of $150.00 per month if switched to a smaller model.


## ❓ FAQ

**Q: How does this tool help reduce AI costs?**
By using `identify_optimization_targets`, you can find features where high costs don't match user engagement, allowing you to switch to more efficient models.

**Q: Can I see which features are using the most models?**
Yes, the `analyze_usage_concentration` tool identifies which features are the primary drivers of AI model consumption.

**Q: How is routing efficiency measured?**
The `get_routing_efficiency_score` tool compares the actual cost incurred by a feature against the theoretical minimum cost of using the most efficient model for that task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-model-usage-analytics](https://vinkius.com/ai-agent-connect/ai-model-usage-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Model Usage Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-model-usage-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Model Usage Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-model-usage-analytics": {
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
