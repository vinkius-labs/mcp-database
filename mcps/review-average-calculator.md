# Review Average Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/review-average-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate arithmetic, weighted, and distributed review metrics.

## Description
This MCP server provides tools to analyze user feedback through various statistical methods. You can use `calculate_simple_average` to find the mean of a set of scores, `calculate_weighted_average` to account for review importance, `filter_reviews_by_date` to isolate feedback within specific timeframes, and `get_rating_distribution` to see how ratings are spread across the scale.


## Available Tools (4)
- **calculate_weighted_average**: Calculates the weighted mean of reviews
- **filter_reviews_by_date**: Filters reviews within a specific timeframe
- **get_rating_distribution**: Gets the distribution of ratings
- **calculate_simple_average**: Calculates the arithmetic mean of a list of scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Review Average Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average of these scores: 4, 5, 3, 5, 2?"

**🤖 AI Agent:**
> The average score is 3.8.

---

**👤 You:**
> "Calculate the weighted average for a score of 5 with weight 2 and a score of 3 with weight 1."

**🤖 AI Agent:**
> The weighted average is 4.33.

---

**👤 You:**
> "Show me the distribution for scores 1, 5, 5, 4, 2."

**🤖 AI Agent:**
> The distribution is: 1: 1, 2: 1, 3: 0, 4: 1, 5: 2.


## ❓ FAQ

**Q: How do I calculate a simple mean?**
Use the `calculate_simple_average` tool by providing an array of numerical scores.

**Q: Can I weight certain reviews more heavily?**
Yes, use `calculate_weighted_average` to assign specific weights to individual reviews.

**Q: How can I see the rating spread?**
The `get_rating_distribution` tool provides a count of reviews for every rating level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/review-average-calculator](https://vinkius.com/en/ai-agent-connect/review-average-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Review Average Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `review-average-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Review Average Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "review-average-calculator": {
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
