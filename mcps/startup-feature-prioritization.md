# Startup Feature Prioritization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startup-feature-prioritization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Prioritize product features using the RICE framework.

## Description
This MCP server provides tools to quantify and rank product features using the RICE (Reach, Impact, Confidence, Effort) framework. It allows product managers to calculate individual scores with `calculate_rice_score`, generate ranked lists via `get_feature_prioritization`, and build execution plans with `get_roadmap_recommendation`. You can also filter features using `search_features_by_metric` to find high-impact or low-effort opportunities.


## Available Tools (4)
- **calculate_rice_score**: Calculates the individual RICE score for a specific feature
- **get_feature_prioritization**: You can optionally provide an alignment weight to boost strategic features.

Generates a ranked list of features based on their RICE scores and strategic alignment
- **get_roadmap_recommendation**: Optionally include dependencies to ensure prerequisites are scheduled first.

Provides a sequential execution plan that respects dependencies and priority
- **search_features_by_metric**: Filters and retrieves features based on specific performance or cost criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Feature Prioritization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RICE score for a feature with 500 reach, 3 impact, 0.8 confidence, and 2 months of effort."

**🤖 AI Agent:**
> The RICE score for this feature is 600.

---

**👤 You:**
> "Show me a ranked list of all features."

**🤖 AI Agent:**
> 1. Feature A (Score: 1200)
2. Feature B (Score: 850)
3. Feature C (Score: 400)

---

**👤 You:**
> "Find features that require less than 3 person-months of effort."

**🤖 AI Agent:**
> The following features meet your criteria: Feature B and Feature D.


## ❓ FAQ

**Q: How is the RICE score calculated?**
The score is calculated by multiplying Reach, Impact, and Confidence, then dividing the result by Effort.

**Q: Can I account for feature dependencies in the roadmap?**
Yes, when using `get_roadmap_recommendation`, you can set the dependency flag to ensure prerequisites are scheduled before the features that depend on them.

**Q: How do I boost features that align with my business goals?**
You can use the `alignmentWeight` parameter in `get_feature_prioritization` to apply a multiplier to features that have high strategic relevance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startup-feature-prioritization](https://vinkius.com/en/ai-agent-connect/startup-feature-prioritization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Feature Prioritization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-feature-prioritization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Feature Prioritization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-feature-prioritization": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
