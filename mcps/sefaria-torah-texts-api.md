# Sefaria Torah Texts API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sefaria-torah-texts-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access sacred texts — audit Torah, Talmud, and library via AI.

## Description
Empower your AI agent to orchestrate your entire religious research and textual auditing workflow with the **Sefaria Torah Texts API**, the comprehensive source for Jewish sacred literature. By connecting Sefaria to your agent, you transform complex scriptural searches into a natural conversation. Your agent can instantly retrieve texts by reference, audit library indices, and query daily reading calendars without you ever touching a physical book. Whether you are conducting academic research or managing daily study constraints, your agent acts as a real-time theological consultant, ensuring your data is always verified and precise.

### What you can do

- **Text Auditing** — Retrieve high-resolution sacred texts by reference (e.g., Genesis 1:1) and maintain a clear view of bilingual content (Hebrew and English).
- **Index Oversight** — Audit the comprehensive library index to understand the thematic distribution of thousands of years of literature instantly.
- **Calendar Discovery** — Query the daily reading schedule, including Parashah and Daf Yomi, to assist in study planning.
- **Metadata Intelligence** — Retrieve unique text identifiers and category markers to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your theological research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (Sefaria is a free and open service)
3. Start managing your scriptural intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Scholars & Educators** — monitor textual data and retrieve official metadata straight from your workflow.
- **Students & Researchers** — verify citations and audit literary patterns without manual searching.
- **Daily Learners** — perform rapid audits of daily readings and identify relevant sacred markers through natural language.
- **Operations Leads** — automate theological data querying to orchestrate cross-functional educational teams smoothly.


## Available Tools (5)
- **check_api_status**: Check if the Sefaria service is operational
- **get_daily_reading_calendar**: Get the daily reading schedule (Parashah, Daf Yomi, etc.)
- **get_sacred_text**: Get a specific sacred text by reference (e.g., Genesis 1:1, Pirkei Avot 1:1)
- **list_library_index**: List all books and categories available in the Sefaria database
- **search_sacred_texts**: Search for keywords or phrases across the entire Sefaria library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sefaria Torah Texts API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get text for 'Genesis 1:1' using Sefaria."

**🤖 AI Agent:**
> I've retrieved the text for Genesis 1:1! In English: "In the beginning God created the heaven and the earth." In Hebrew: "בְּרֵאשִׁית בָּרָא אֱלֹהִים אֵת הַשָּׁמַיִם וְאֵת הָאָרֶץ". Would you like the full chapter metadata or the next verse?

---

**👤 You:**
> "What is the Daf Yomi for today?"

**🤖 AI Agent:**
> I've retrieved the reading calendar for today! The current Daf Yomi is identified as [Tractate and Page]. I can provide the full text and commentary links for this section if you'd like.

---

**👤 You:**
> "Search for texts about 'justice' in Sefaria."

**🤖 AI Agent:**
> I've identified several passages about justice in the Sefaria library! Notable entries include verses from Deuteronomy and the Prophets. I can provide the full citations and bilingual text for each of these matches.


## ❓ FAQ

**Q: Is an API Key required for Sefaria API?**
No. Sefaria provides a free public API for non-commercial use. This server works out of the box without any static credentials required.

**Q: What languages are the texts available in?**
The Sefaria API primarily provides texts in their original Hebrew or Aramaic along with professional English translations.

**Q: Can the agent show the weekly Parashah?**
Yes. The `get_daily_reading_calendar` tool retrieves the official weekly Torah portion (Parashah) and other daily study markers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sefaria-torah-texts-api](https://vinkius.com/mcp/sefaria-torah-texts-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sefaria Torah Texts API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sefaria-torah-texts-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sefaria Torah Texts API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sefaria-torah-texts-api": {
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
