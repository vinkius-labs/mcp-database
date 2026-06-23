# Deterministic Reading Project Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-reading-project-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform your AI into a hyper-efficient literary project manager. Analyze reading lists, calculate strict algorithmic completion times, and generate momentum-based reading sequences instantly.

## Description
Managing extensive reading backlogs (like research papers, tech books, or documentation) is a common productivity bottleneck. LLMs struggle with accurately summing pages, tracking percentages, or estimating true time-to-completion because they guess math instead of calculating it. The Reading Project Manager MCP resolves this by ingesting your list and processing it through a strict V8 algorithmic engine.

### The Superpowers
- **Momentum-Based Sequencing (Snowball Method):** Automatically sorts your reading queue to prioritize books you are closest to finishing, followed by the shortest unread books to build rapid psychological momentum.
- **Precision Time Estimation:** Calculates exact hours remaining based on total unread pages and your specific reading speed (Words Per Minute), assuming standard 300-word academic pages.
- **Holistic Progress Analytics:** Generates a real-time JSON dashboard summarizing total completion percentage, pages read vs. unread, and active pipeline statuses.
- **Zero-Dependency Architecture:** Pure JS runtime execution guarantees absolute microsecond speed without any massive external NPM dependencies.


## Available Tools (1)
- **analyze_reading_list**: Provide the items array as a JSON string, ensuring all required fields are present.

Analyzes an array of reading items to generate comprehensive progress reports, estimate exact completion times (based on WPM), and construct an optimized reading sequence using the Snowball Method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Reading Project Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my book queue and tell me how many hours I have left."

**🤖 AI Agent:**
> Using the analyze_reading_list tool: You have 1,200 pages left across 4 unread books. At 250 WPM, it will take approximately 24 hours of focused reading.

---

**👤 You:**
> "What book should I read next to build momentum?"

**🤖 AI Agent:**
> Using the analyze_reading_list tool: Based on the Snowball sequence, you should finish 'The Lean Startup' (only 40 pages left), followed immediately by your shortest unread book, 'Who Moved My Cheese' (96 pages).

---

**👤 You:**
> "Calculate my progress across these 15 research papers."

**🤖 AI Agent:**
> Using the analyze_reading_list tool: Your diagnostic shows you are 45.2% complete overall, having finished 7 papers entirely and being halfway through another.


## ❓ FAQ

**Q: How does it estimate the time remaining?**
The algorithmic engine multiplies your remaining unread pages by an industry-standard 300 words-per-page. It then divides that massive word count by your specific reading speed (defaulting to 250 Words Per Minute) to output an exact hour count.

**Q: What is the Snowball Method sequence?**
It is a psychological productivity framework. The algorithm sorts your 'reading' books by how close you are to finishing them. For completely unread books, it sorts them from shortest to longest. This guarantees you secure 'quick wins' fast to build reading momentum.

**Q: Can it process dozens of books at once?**
Yes. Because it uses pure JSON and mathematical mapping without LLM token limits, it can instantly evaluate libraries containing thousands of entries without any calculation hallucination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-reading-project-manager](https://vinkius.com/mcp/deterministic-reading-project-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Reading Project Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-reading-project-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Reading Project Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-reading-project-manager": {
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
