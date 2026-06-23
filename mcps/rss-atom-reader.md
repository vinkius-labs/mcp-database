# RSS / Atom Reader MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rss-atom-reader)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI assistant to any RSS or Atom feed worldwide to fetch news, updates, and articles instantly within your chat interface.

## Description
Connect your conversational assistant to read and analyze data natively from any **RSS or Atom feed**. This simple but powerful integration acts as an instant news parser, transforming massive external XML news feeds into summarized text right inside the interface.

### What you can do

- **Scan Any Feed Instantly** — Point the assistant directly to a custom URL (`read_feed`) to retrieve the top 10 to 50 latest news articles without changing tabs or formatting logic.
- **Configure a Default Feed** — Skip typing URLs and set up an overarching operational default source (`read_default_feed`), simplifying daily check-ins like reading standard tech blogs, release notes, or internal company updates automatically parsed.

### How it works

1. Install the standalone RSS Reader module into your native MCP framework seamlessly.
2. (Optional) In the configuration parameters securely locked below, deposit a standard default RSS/XML link representing a blog, journal, or feed you consistently monitor.
3. Chat with the AI: "List the latest 5 updates from our default feed." or "Extract the top articles from this specific http://site.com/rss address natively."

### Who is this for?

- **Analysts & Researchers** — Bypass paywalled complex news tools and rapidly synthesize daily technology or market trends directly interacting conversationally.
- **Operators & Tech Lead Teams** — Automatically fetch the latest release logs internally and feed them textually into algorithmic summaries.
- **Everyone** — Build custom organic micro-dashboards logically extracting new data continuously inside your own chat.


## Available Tools (2)
- **read_default_feed**: Reads the default configured RSS feed
- **read_feed**: Specify the URL and an optional limit.

Reads and parses an RSS or Atom feed from a provided URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RSS / Atom Reader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Determine the top 5 article posts sourced natively securely traversing strictly http://dummy.com/rss."

**🤖 AI Agent:**
> I securely read the feed natively using the `read_feed` call strictly passing 'http://dummy.com/rss'. Here are your 5 parsed structured news headlines:
1. Tech Launch Event Completed...
[...]

---

**👤 You:**
> "Read the latest updates from my default feed."

**🤖 AI Agent:**
> I've fetched the latest 10 articles from your default feed. Here are the top headlines:
1. New Vinkius MCP Server Released
2. The Future of Conversational AI
3. Best Practices for Tool Integration
Do you want me to summarize any of these in detail?

---

**👤 You:**
> "Fetch the single most recent article from the tech news feed."

**🤖 AI Agent:**
> The most recent article from the tech news feed is 'Quantum Computing Breakthrough'. It was published 2 hours ago. The summary states scientists have achieved a new milestone in qubit stability. Should I provide the full link?


## ❓ FAQ

**Q: Are specific RSS/Atom formats parsed incorrectly?**
The tool uses modern XML parsers logically built to consume seamlessly both widely structured and legacy encoded Atom and standard RSS payloads perfectly consistently directly from organic sources mitigating rendering discrepancies.

**Q: What is the difference between `read_feed` and `read_default_feed`?**
`read_feed` requires you to provide a URL each time you call it. `read_default_feed` uses a pre-configured URL so you can check your favorite source without repeating the address every time.

**Q: How many articles can I retrieve per request?**
You can fetch between 1 and 50 items per call using the `limit` parameter. The default is 10 if no limit is specified.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rss-atom-reader](https://vinkius.com/mcp/rss-atom-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RSS / Atom Reader** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rss-atom-reader` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RSS / Atom Reader** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rss-atom-reader": {
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
