# NDL Japan Library Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ndl-japan-library-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Japan's National Diet Library as an MCP: search 100M+ records — books, journals, dissertations, digitized Meiji/Edo classics — by title, author, publisher or ISBN, with NDL viewer links. Keyless.

## Description
The **National Diet Library (NDL)** — Japan's national library and one of the largest collections on Earth — as a single MCP server.

### What you can do
- **Search 100M+ records** — every book, journal article, dissertation, map and government document catalogued in Japan, matched by title, author, publisher or any field
- **ISBN lookup** — authoritative Japanese bibliographic data for any book: exact kanji title, author, publisher, dates, volumes/pages, subjects
- **Digitized treasures** — the NDL Digital Collections hold free scans of Meiji and Edo era books, ukiyo-e, historical documents and pre-war journals

### What lives here
The memory of Japan: 400 years of printing, every PhD thesis since Japan had universities, the complete congressional library of the Diet, and a digitization program that made centuries of rare Japanese books free to read online.

### Who is this for?
Researchers, translators, historians, bibliographers, librarians, book collectors and AI agents that need authoritative Japanese bibliographic data or want to locate digitized Japanese primary sources.


## Available Tools (3)
- **find_book_by_isbn**: The fastest way to get authoritative Japanese bibliographic data for a book. NOTE: the NDL API requires the hyphenated ISBN form — this tool inserts the hyphens automatically.

Look up one book in the NDL catalog by ISBN-13 or ISBN-10
- **search_national_library**: Query modes: title= (book/article titles), any= (all fields), creator= (author), publisher=. Japanese terms work best; English also matches many records. Returns title, author, publisher, date, ISBN, subjects, categories and NDL page URL. NOTE: the API has no server-side pagination — set cnt to the window you need (max ~200).

Search the National Diet Library of Japan: 100M+ books, journals, dissertations, digitized classics and government documents
- **search_digitized_history**: Ideal for 明治/江戸 era books, historical documents, old maps and journals that are digitized and free to read. Returns digitized item metadata with NDL viewer links.

Search NDL Digitized Collections: scanned Japanese classics, Meiji-era books, rare documents (all free)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NDL Japan Library Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find books about ramen in Japan's national library"

**🤖 AI Agent:**
> 📚 **NDL search: ラーメン (title)**

10,983 records. Top hits:
- 嗚呼!このラーメンがうまい : 首都圏版 — guide to the Kanto's best bowls
- 嗚呼!このラーメンがうまい : 関西版 — Kansai edition

From 1970s food culture to modern academic studies of ramen globalization. Want a filtered look at the academic titles?

---

**👤 You:**
> "Look up ISBN 978-4-12-390001-1 in the NDL catalog"

**🤖 AI Agent:**
> 📖 **ISBN lookup via NDL**

Title: 数え方の辞典 (Dictionary of Counting Words)
Author: 飯田朝子 · Publisher: 朝日新聞出版

Japanese counters (本/枚/匹...) are famously hard — this is the standard reference. I can pull related counter-dictionary titles too.

---

**👤 You:**
> "Are there digitized Meiji-era books about the railway?"

**🤖 AI Agent:**
> 🎴 **NDL Digitized Collections: 明治 鉄道**

Yes! Free scans include:
- Meiji railway construction reports (official documents)
- Early travel guides with train timetables from 1889
- Illustrated books on the Tokaido line

All readable in the NDL viewer. I can search a specific year or region next.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The NDL Search OpenSearch API is fully public — all tools work without authentication.

**Q: Does the API support pagination?**
The NDL OpenSearch endpoint has no server-side pagination (tested: pagenum/first/start params are ignored). Each call returns the top 'cnt' results (up to ~200). For deeper results, refine the query terms instead of paging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ndl-japan-library-search](https://vinkius.com/en/ai-agent-connect/ndl-japan-library-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NDL Japan Library Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ndl-japan-library-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NDL Japan Library Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ndl-japan-library-search": {
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
