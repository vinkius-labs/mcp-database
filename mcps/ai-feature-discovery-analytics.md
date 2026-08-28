# AI Feature Discovery Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-discovery-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Measure and optimize how users find and engage with your AI features.

## Description
This MCP server provides a specialized analytics engine for SaaS products to measure the effectiveness of AI feature launches. It calculates core metrics like discovery rate, evaluates the performance of different discovery channels, and analyzes the velocity of user adoption. By using tools like `calculate_discovery_metrics` and `analyze_discovery_velocity`, product teams can identify friction in UI placement and generate actionable acceleration strategies to improve feature awareness and engagement.


## Available Tools (4)
- **calculate_discovery_metrics**: Provides the fundamental health score of an AI feature's launch
- **evaluate_channel_performance**: Determines which marketing or UI paths are most successful at driving engagement
- **analyze_discovery_velocity**: Measures the speed of adoption and identifies delays in feature awareness
- **generate_acceleration_strategy**: Provides actionable advice to improve discovery based on current performance gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature Discovery Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current discovery rate if 1000 users saw the feature and 250 tried it?"

**🤖 AI Agent:**
> The discovery rate is 25%.

---

**👤 You:**
> "How fast are users finding the feature? The discovery days are [2, 5, 3, 8, 1] and the UI placement is primary."

**🤖 AI Agent:**
> The average days to discovery is 3.8 days.

---

**👤 You:**
> "Give me a strategy for a feature with a 10% discovery rate, high UI friction, and low promotion intensity."

**🤖 AI Agent:**
> Prioritize improving UI placement to reduce friction before increasing promotional efforts.


## ❓ FAQ

**Q: What is the discovery rate?**
The discovery rate is the percentage of users who successfully identified and attempted to use an AI feature out of the total group exposed to it, calculated via `calculate_discovery_metrics`.

**Q: How can I improve my feature adoption?**
You can use `generate_acceleration_strategy` to receive specific, actionable advice based on your current discovery rate, UI friction, and promotion intensity.

**Q: Can I compare different marketing channels?**
Yes, the `evaluate_channel_performance` tool allows you to compare the effectiveness of various channels like Modals, Tooltips, or Email.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-discovery-analytics](https://vinkius.com/ai-agent-connect/ai-feature-discovery-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature Discovery Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-discovery-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature Discovery Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-discovery-analytics": {
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
