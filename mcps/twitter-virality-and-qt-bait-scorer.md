# Twitter Virality and QT Bait Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twitter-virality-and-qt-bait-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Quantify the 'Quote Tweet' incentive and virality potential of a tweet using linguistic pattern matching.

## Description
The Twitter Virality and QT Bait Scorer uses deterministic language markers to identify the structural potential of a tweet to trigger Quote Tweets and high-engagement virality. By analyzing features like contrarian statement density, hot-take index, controversy quotient, and 'takes vs facts' ratio, it provides an objective metric for engagement prediction. Use `analyze_virality` to assess punctuation diversity and sentence variety, or use `analyze_qt_bait` to evaluate the provocation potential of a tweet.


## Available Tools (2)
- **analyze_qt_bait**: Analyze a tweet for QT bait potential
- **analyze_virality**: Analyze a tweet for virality potential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twitter Virality and QT Bait Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this tweet for virality: 'Unpopular opinion: the best way to work is remote. Actually, it's not even a choice.'"

**🤖 AI Agent:**
> The tweet has a high virality score due to significant punctuation diversity and sentence variety.

---

**👤 You:**
> "Evaluate the QT bait potential of this tweet: 'I think we should always be honest. It is a fact that truth is essential.'"

**🤖 AI Agent:**
> The tweet shows low provocation potential with a low density of contrarian markers and a high ratio of facts to takes.

---

**👤 You:**
> "Check the engagement score for: 'Wrong! You are completely mistaken about this topic.'"

**🤖 AI Agent:**
> The tweet has a high provocation index and significant contrarian density.


## ❓ FAQ

**Q: What metrics does the tool use to calculate virality?**
The `analyze_virality` tool calculates scores based on punctuation diversity and sentence variety within the provided text.

**Q: How does it identify 'QT bait' for a tweet?**
The `analyze_qt_bait` tool identifies patterns like contrarian density and provocation index to determine how likely a tweet is to trigger Quote Tweets.

**Q: Is this tool for sentiment analysis?**
No, it is a deterministic engine that uses pattern matching to identify linguistic architectures associated with engagement-driving behavior.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twitter-virality-and-qt-bait-scorer](https://vinkius.com/mcp/twitter-virality-and-qt-bait-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twitter Virality and QT Bait Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twitter-virality-and-qt-bait-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twitter Virality and QT Bait Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twitter-virality-and-qt-bait-scorer": {
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
