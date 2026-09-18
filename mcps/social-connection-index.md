# Social Connection Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/social-connection-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Measures social connection quality and quantity to assess overall social health.

## Description
This MCP connects AI agents to tools that evaluate an individual's social fabric. By analyzing the balance between relationship quality and quantity, it provides a comprehensive view of social well-being. Use `get_connection_score` to find the aggregate integration score, `assess_loneliness_risk` to identify potential isolation, `calculate_relationship_diversity` to check the variety of social circles, and `get_social_health_recommendations` for actionable guidance.


## Available Tools (4)
- **calculate_relationship_diversity**: Evaluates the breadth and variety of an individual's social ecosystem
- **get_connection_score**: Calculates the aggregate social connection index score for an individual
- **get_social_health_recommendations**: Provides personalized guidance to improve or maintain social well-being
- **assess_loneliness_risk**: Determines the likelihood of an individual experiencing social isolation or loneliness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Connection Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my social connection score with 3 close relationships, 10 weekly interactions, and a community involvement score of 5."

**🤖 AI Agent:**
> Your social connection index score is 45, indicating a healthy level of social integration.

---

**👤 You:**
> "Assess my loneliness risk. I report a loneliness score of 8, have 1 close relationship, and 2 weekly interactions."

**🤖 AI Agent:**
> Your loneliness risk is High due to the high self-reported loneliness score and low number of close relationships.

---

**👤 You:**
> "What is my relationship diversity if I have 5 close relationships, 10 casual acquaintances, and 2 community members?"

**🤖 AI Agent:**
> Your relationship diversity score is 7.5, showing a well-distributed social ecosystem across all tiers.


## ❓ FAQ

**Q: How is the social connection score calculated?**
The score is calculated using `get_connection_score`, which weights close relationships and community involvement while using weekly interactions as a secondary factor.

**Q: Can this tool help identify loneliness risk?**
Yes, by using `assess_loneliness_risk`, the tool compares self-reported loneliness levels against actual social interaction counts to determine risk levels.

**Q: What kind of advice does it provide?**
The `get_social_health_recommendations` tool provides personalized advice, such as suggesting ways to deepen existing bonds or seek more community involvement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/social-connection-index](https://vinkius.com/en/ai-agent-connect/social-connection-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Connection Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-connection-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Connection Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-connection-index": {
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
