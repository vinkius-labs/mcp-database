# e-Gov Japan Laws MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/e-gov-japan-laws)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Japan's official legislation portal as an MCP: browse all 18,000+ acts, cabinet orders and ordinances, fetch full structured text (chapters > articles > paragraphs), extract single articles or search keywords inside laws — keyless.

## Description
**e-Gov** is the Japanese government's official legal portal — every law in force in Japan, as a single MCP server.

### What you can do
- **Browse the catalog** — the Constitution + all acts (~9,000), cabinet orders (~2,100), imperial orders (~2,400) and ministerial ordinances (~4,500), each with law ID, number and promulgation date
- **Fetch full structured text** — complete law as a clean hierarchy: Law > Chapter > Article > Paragraph > Sentence
- **Get the outline first** — chapters and article titles without the text, the fast way to understand a law's coverage
- **Extract one article** — "what does Article 29 of the Constitution say", answered with the exact promulgated text
- **Search inside laws** — find where a topic is regulated: 消費税 (consumption tax), 労働 (labour), 選挙 (elections) across every article of a law

### Why it matters
Japanese law text is famously opaque to outsiders: kanji numbering, era-based dates (令和/Reiwa), mixed act/order hierarchy. This MCP gives you the authoritative source — the same text courts and companies cite — in structured form an AI can navigate.

### Who is this for?
Legal-tech builders, compliance teams, researchers, translators, journalists and AI agents that need the actual text of Japanese law.


## Available Tools (5)
- **get_law**: Use law_id from list_laws (e.g. 321CONSTITUTION = the Constitution). Large laws can be several hundred KB. Text is Japanese.

Get the FULL structured text of a Japanese law (articles, chapters, provisions)
- **list_laws**: Categories: 1=Constitution + Acts (all laws, ~9000), 2=Cabinet Orders (~2100), 3=Imperial Orders (~2400), 4=Ministerial Ordinances (~4500). Each entry: law_id (use in get_law), law_name, law_number, promulgation date. Japanese text. Use query_terms to filter client-side — the API has no server-side search.

List Japanese laws by category (constitution, acts, imperial orders, ministerial ordinances) with law IDs
- **get_law_outline**: The fast way to see what a law covers before fetching specific articles.

Get the structural outline of a law WITHOUT the full text (chapters + article titles)
- **get_law_article**: For "what does Article 29 of the Constitution say". Tip: article Num attribute follows the kanji numbering order — use get_law_outline first to map article numbers.

Extract ONE article (or chapter) of a Japanese law with its full text
- **search_law_articles**: Japanese keyword required (e.g. 消費税 for consumption tax, 労働 for labour, 選挙 for elections).

Search every article of a law for a keyword (finds where a topic is regulated)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **e-Gov Japan Laws** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What does Article 29 of the Japanese Constitution say?"

**🤖 AI Agent:**
> ⚖️ **Constitution (日本国憲法) — Article 29**

Paragraph 1: The right to own or to hold property is inviolable.
Paragraph 2: Property rights shall be defined by law, in conformity with the public welfare.
Paragraph 3: Private property may be taken for public use upon just compensation therefor.

Sources straight from e-Gov (321CONSTITUTION). Want the preceding property-rights articles or the English context?

---

**👤 You:**
> "Where is consumption tax regulated? Search the consumption tax act for 消費税"

**🤖 AI Agent:**
> 🔎 **Consumption Tax Act — keyword search 消費税**

Found 47 matching articles. Key ones:
- Article 4 (課税物件): taxable goods and transactions
- Article 28: tax rate application per category
- Article 57: export exemptions

I can pull the full text of any of these articles or search another law.

---

**👤 You:**
> "Give me the outline of Japan's Labour Standards Act"

**🤖 AI Agent:**
> 📋 **Labour Standards Act (労働基準法) — outline**

Chapter 1: General provisions (arts. 1-13)
Chapter 2: Labour contracts (14-18)
Chapter 3: Wages (24-26) · Chapter 4: Working hours (32-40) · Chapter 5: Safety and health…

13 chapters, ~120 articles. Want the full text of the working-hours chapter?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The e-Gov Laws API is fully public — list, full text, outline, article extraction and keyword search all work without authentication.

**Q: How do I find the law_id I need?**
Use list_laws with query_terms — e.g. category 1 with 労働 (labour) returns every act whose name contains it. Law IDs look like 321CONSTITUTION or 平成五年法律第八十九号 encoded as IDs. There is no server-side keyword search in the e-Gov API, so filtering happens client-side.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/e-gov-japan-laws](https://vinkius.com/en/ai-agent-connect/e-gov-japan-laws)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **e-Gov Japan Laws** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `e-gov-japan-laws` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **e-Gov Japan Laws** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "e-gov-japan-laws": {
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
