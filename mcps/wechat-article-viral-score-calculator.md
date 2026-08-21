# WeChat Article Viral Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wechat-article-viral-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Predict the shareability of WeChat articles using structural and topical metrics.

## Description
This MCP server provides a deterministic engine to estimate the viral potential of WeChat Official Account articles. By analyzing structural elements like paragraph density and image count via `get_readability_score`, matching content against trending topics with `get_keyword_match_score`, and evaluating release timing with `get_posting_time_score`, it produces a comprehensive `calculate_total_viral_score`. It helps creators optimize content for the WeChat ecosystem's unique consumption patterns.


## Available Tools (4)
- **calculate_total_viral_score**: Provides the final, single metric representing the article's total viral potential
- **get_keyword_match_score**: Determines how well the article aligns with current trending topics
- **get_posting_time_score**: Predicts the impact of the article's release time on its initial reach
- **get_readability_score**: Evaluates the structural quality of the article to determine how consumable it is


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Article Viral Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the viral score for an article with 10 paragraphs, 4 images, matching 2 out of 5 trending keywords, and posted at 19:00."

**🤖 AI Agent:**
> The total viral score is 74.0. (Readability: 80, Keyword Match: 40, Posting Time: 100).

---

**👤 You:**
> "What is the readability score for an article with 5 paragraphs and 2 images?"

**🤖 AI Agent:**
> The readability score is 90.

---

**👤 You:**
> "How much does posting at 12:30 contribute to the score?"

**🤖 AI Agent:**
> Posting at 12:30 results in an optimal posting time score of 80.


## ❓ FAQ

**Q: How is the readability score calculated?**
The `get_readability_score` tool starts with a baseline of 100, subtracts 2 points for every paragraph, and adds 5 points for every image, capped at 100.

**Q: What is the best time to post for a higher score?**
Using `get_posting_time_score`, you can see that publishing between 18:00 and 20:00 yields the highest score (100), followed by the lunch window (12:00-13:00) which yields 80.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wechat-article-viral-score-calculator](https://vinkius.com/ai-agent-connect/wechat-article-viral-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeChat Article Viral Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wechat-article-viral-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeChat Article Viral Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wechat-article-viral-score-calculator": {
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
