# Wine PR Sentiment Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-pr-sentiment-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Quantify media impact, brand health, and reputation risks for wine brands.

## Description
This MCP server provides specialized sentiment intelligence for wine brands. It connects AI agents to media data to calculate the Brand Health Index, evaluate PR campaign impact, and monitor reputation signals. Use `get_sentiment_summary` to analyze brand tone, `calculate_brand_health` to assess reputation strength, `evaluate_pr_impact` to measure campaign success, `monitor_reputation_signals` to detect risks or opportunities, and `get_share_of_voice` to compare market presence against competitors.


## Available Tools (5)
- **calculate_brand_health**: Calculate the Brand Health Index (BHI) for a wine brand
- **evaluate_pr_impact**: Evaluate the impact of a PR campaign
- **get_sentiment_summary**: Get the current overall sentiment of a wine brand
- **get_share_of_voice**: Get the Share of Voice (SOV) for a brand in a specific category
- **monitor_reputation_signals**: Monitor for immediate reputation risks or opportunities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine PR Sentiment Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current sentiment for Chateau Reserve over the last 7 days?"

**🤖 AI Agent:**
> The average sentiment score for Chateau Reserve over the last 7 days is 0.75, with 45 positive mentions, 5 neutral mentions, and 2 negative mentions.

---

**👤 You:**
> "How successful was the Summer Rosé campaign from 2024-06-01 to 2024-06-30?"

**🤖 AI Agent:**
> The Summer Rosé campaign achieved an impact score of 82, with a reach lift of 15,000 and a sentiment shift of +0.15.

---

**👤 You:**
> "Check for any reputation risks for Vintage Vine."

**🤖 AI Agent:**
> No immediate reputation risks were detected for Vintage Vine; the current Share of Voice trend is stable.


## ❓ FAQ

**Q: How does the Brand Health Index work?**
The `calculate_brand_health` tool determines the index by multiplying the sentiment score by the logarithm of the total reach, normalized against industry benchmarks.

**Q: Can I track my market share in specific wine categories?**
Yes, you can use `get_share_of_voice` to see your brand's percentage of the conversation within categories like Rosé or Merlot compared to competitors.

**Q: How are reputation risks identified?**
The `monitor_reputation_signals` tool identifies risks when negative sentiment reach exceeds your specified sensitivity threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-pr-sentiment-intelligence](https://vinkius.com/en/ai-agent-connect/wine-pr-sentiment-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine PR Sentiment Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-pr-sentiment-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine PR Sentiment Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-pr-sentiment-intelligence": {
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
