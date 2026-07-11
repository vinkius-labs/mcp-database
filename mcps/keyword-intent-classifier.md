# Keyword Intent Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keyword-intent-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Categorize search keywords by intent, length, and marketing funnel stage.

## Description
The Keyword Intent Classifier connects AI agents to a rule-based engine that analyzes search queries. Using `classify_keyword` and `batch_classify_keywords_tool`, you can determine if a keyword is Informational, Navigational, Commercial, or Transactional. The tool also identifies keyword length distribution (Head, Body, Long-tail) and maps keywords to the appropriate marketing funnel stage: TOFU, MOFU, or BOFU. This is essential for SEO strategy and content planning.


## Available Tools (2)
- **classify_keywords_batch**: Classify a list of keywords in bulk
- **classify_keyword**: Classify a single keyword into an intent category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keyword Intent Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify the keyword 'best running shoes for marathons'"

**🤖 AI Agent:**
> Intent: Commercial, Confidence Score: 0.85, Length Category: Long-tail, Funnel Stage: MOFU

---

**👤 You:**
> "What is the intent of 'how to bake a cake'?"

**🤖 AI Agent:**
> Intent: Informational, Confidence Score: 0.9, Length Category: Body, Funnel Stage: TOFU

---

**👤 You:**
> "Analyze the keyword 'buy iphone'"

**🤖 AI Agent:**
> Intent: Transactional, Confidence Score: 0.95, Length Category: Head, Funnel Stage: BOFU


## ❓ FAQ

**Q: How does the classification work?**
The engine uses a predefined lexicon of intent-signal modifiers like 'how to', 'buy', or 'best' to assign categories and confidence scores.

**Q: What are the funnel stages?**
Keywords are mapped to TOFU (Informational), MOFU (Commercial/Navigational), or BOFU (Transactional) based on their detected intent.

**Q: Can I process multiple keywords at once?**
Yes, you can use the `batch_classify_keywords_tool` to analyze an array of keywords and receive a summary of their distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keyword-intent-classifier](https://vinkius.com/mcp/keyword-intent-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keyword Intent Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keyword-intent-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keyword Intent Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keyword-intent-classifier": {
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
