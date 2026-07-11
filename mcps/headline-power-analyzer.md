# Headline Power Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/headline-power-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze headlines for power words, emotional impact, sentiment, and platform compliance.

## Description
The Headline Power Analyzer is a specialized linguistic engine designed to optimize your marketing copy. By connecting AI agents to this MCP server, you can perform deep analysis on any headline or title string. Use `analyze_headline_linguistics` to identify high-impact power words and calculate the Emotional Marketing Value (EMV) percentage based on word composition. The `get_sentiment_analysis` tool allows you to determine the emotional tone and polarity of your text, ensuring it aligns with your brand voice. Additionally, the `check_platform_compliance` tool provides critical structural feedback by estimating pixel width and character counts for major platforms like Google Ads, Meta Ads, X (formerly Twitter), and email subject lines, alerting you to potential truncation before you publish.


## Available Tools (3)
- **check_platform_compliance**: Checks if a headline will be truncated on major platforms
- **get_sentiment_analysis**: Analyzes the emotional tone and sentiment polarity of a headline
- **analyze_headline_linguistics**: Analyzes the linguistic composition and word-type balance of a headline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Headline Power Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this headline for power words: 'Unbelievable secrets to massive wealth!'"

**🤖 AI Agent:**
> Power words found: Unbelievable, secrets, massive, wealth. The calculated EMV is 45%.

---

**👤 You:**
> "What is the sentiment of 'I am so happy today'?"

**🤖 AI Agent:**
> The sentiment analysis shows a Positive tone with a polarity score of 0.85.

---

**👤 You:**
> "Will this headline fit on Google Ads: 'This is an extremely long and detailed headline that will definitely be truncated by the platform limits.'"

**🤖 AI Agent:**
> The status for Google Ads RSA is Truncated. The character count exceeds the allowed limit.


## ❓ FAQ

**Q: How can I check if my headline is too long for Twitter?**
You can use the `check_platform_compliance` tool to verify the character count and estimated pixel width against platform-specific constraints.

**Q: What is EMV in this context?**
EMV stands for Emotional Marketing Value. It is a percentage calculated by analyzing the ratio of emotional words to the total word count in your headline.

**Q: Does this tool support languages other than English?**
The current version of the linguistic analysis engine is optimized for English-language headlines and uses an English-based lexicon.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/headline-power-analyzer](https://vinkius.com/mcp/headline-power-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Headline Power Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `headline-power-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Headline Power Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "headline-power-analyzer": {
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
