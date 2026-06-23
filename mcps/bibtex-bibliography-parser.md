# BibTeX Bibliography Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bibtex-bibliography-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Parse academic .bib bibliography files into structured JSON. Let your AI format citations in APA, IEEE, or Chicago style instantly local.

## Description
Students and researchers manage hundreds of references in .bib files. Asking Claude to reformat them manually is error-prone. This MCP parses the entire BibTeX structure using deterministic regex (zero dependencies) and delivers clean JSON entries with type, citation key, and all fields.

### The Superpowers

- **Zero Dependencies:** Pure regex parsing, no external libs needed.
- **Type Aggregation:** Instantly shows how many articles, books, and proceedings you have.
- **Citation Ready:** Ask the AI to reformat entries in APA, IEEE, or any style.


## Available Tools (1)
- **parse_bibtex_bibliography**: bib file with academic references. Provide the absolute file path.

Parse a BibTeX .bib bibliography file into structured JSON. Perfect for students and researchers who want to query their references with AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BibTeX Bibliography Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert all entries from 2023 in my .bib to APA format."

**🤖 AI Agent:**
> Here are 12 entries from 2023 reformatted in APA style.

---

**👤 You:**
> "How many articles vs books do I have?"

**🤖 AI Agent:**
> Your bibliography has 85 articles, 12 books, and 8 inproceedings.

---

**👤 You:**
> "Find all references by author 'Smith' in my bibliography."

**🤖 AI Agent:**
> Found 7 entries authored by Smith across years 2018-2024.


## ❓ FAQ

**Q: Does it handle LaTeX special characters?**
It extracts the raw field values as-is. The AI can then interpret or clean LaTeX escapes like \'{e} into proper Unicode.

**Q: How many entries can it handle?**
It caps the output at 200 entries to protect AI context. For larger bibliographies, ask the AI to filter by type or year.

**Q: Can it detect duplicate references?**
The parser extracts all entries. You can then ask the AI: 'Find duplicate titles or DOIs in my bibliography.'


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bibtex-bibliography-parser](https://vinkius.com/mcp/bibtex-bibliography-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BibTeX Bibliography Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bibtex-bibliography-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BibTeX Bibliography Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bibtex-bibliography-parser": {
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
