# Keyword Proximity Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keyword-proximity-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Analyze text to measure the word distance between keywords for SEO relevance.

## Description
The Keyword Proximity Checker is an analytical tool designed to assess semantic relevance for search engine optimization. By calculating the exact number of words separating specific keywords, it helps identify topical density and clusters within a text. Use `get_word_distance` to find the distance between two terms, `evaluate_proximity_status` to check if pairs meet a threshold, or `detect_keyword_clusters` to locate high-density keyword groups.


## Available Tools (3)
- **evaluate_proximity_status**: Determine if specific pairs of keywords meet a predefined proximity threshold
- **detect_keyword_clusters**: Identify clusters where multiple keywords appear near each other
- **get_word_distance**: Calculate the exact number of words separating two specific keywords in a given text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keyword Proximity Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the distance between 'apple' and 'banana' in the text: 'I ate an apple and then a banana.'?"

**🤖 AI Agent:**
> The distance between 'apple' and 'banana' is 3 words.

---

**👤 You:**
> "Check if 'SEO' and 'content' are near in: 'High quality SEO content is vital.' with a max distance of 1."

**🤖 AI Agent:**
> The pair 'SEO - content' has a status of Near with an actual distance of 0.

---

**👤 You:**
> "Find clusters for ['cat', 'dog'] in: 'The cat and dog played.' with window size 3."

**🤖 AI Agent:**
> A cluster was found containing ['cat', 'dog'] starting at index 1 and ending at index 3.


## ❓ FAQ

**Q: How is the word distance calculated?**
The tool calculates the difference between the positions of the keywords and subtracts one. It always finds the shortest possible distance if a keyword appears multiple times.

**Q: What is a keyword cluster?**
A cluster is identified when multiple keywords from your list all appear within a specified `windowSize` range of tokens.

**Q: Can I check multiple keyword pairs at once?**
Yes, using the `evaluate_proximity_status` tool, you can provide a list of keywords and a maximum distance to see which pairs are 'Near' or 'Far'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keyword-proximity-checker](https://vinkius.com/mcp/keyword-proximity-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keyword Proximity Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keyword-proximity-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keyword Proximity Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keyword-proximity-checker": {
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
