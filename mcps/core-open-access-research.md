# CORE (Open Access Research) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/core-open-access-research)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of open access research papers, journals, and repositories directly from your AI agent using the CORE API.

## Description
Connect to **CORE**, the world's largest aggregator of open access research papers. This MCP server allows your AI agent to search, retrieve, and analyze millions of scholarly articles, journals, and institutional repositories through natural conversation.

### What you can do

- **Global Search** — Search across all CORE resources including articles, journals, and repositories using a single text query.
- **Article Retrieval** — Fetch full metadata, version history, and direct PDF download links for specific research papers using CORE IDs.
- **Journal & Repository Discovery** — Search and inspect specific journals by ISSN or explore institutional repositories to find authoritative sources.
- **OAI Resolution** — Resolve Open Archives Initiative (OAI) identifiers to access original metadata and repository pages.
- **Deep Metadata Inspection** — Analyze article history and updates to ensure you are working with the latest scientific information.

### How it works

1. Subscribe to this server
2. Enter your CORE API Key
3. Start researching directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find relevant papers and download PDFs without leaving your writing or coding environment.
- **Students** — gather citations, explore related research history, and find open access versions of paywalled content.
- **Data Scientists** — access a massive corpus of open access metadata for literature reviews and scientific data analysis.


## Available Tools
- **get_article_history**: Get the history of an article
- **get_article_pdf**: Get the PDF download URL for an article
- **get_article**: Get a specific article by CORE ID
- **get_journal**: Get a specific journal by ISSN
- **get_repository**: Get a specific repository by ID
- **global_search**: Global search across CORE
- **resolve_oai**: Resolve an OAI identifier
- **search_articles**: Search for articles
- **search_journals**: Search for journals
- **search_repositories**: Search for repositories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CORE (Open Access Research)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search CORE for the latest research on transformer architectures in NLP."

**🤖 AI Agent:**
> I've performed a global search on CORE. I found several high-impact papers, including 'Attention is All You Need' and recent variants. Would you like the CORE IDs or PDF links for the top 3 results?

---

**👤 You:**
> "Get the PDF download link for the article with CORE ID 123456."

**🤖 AI Agent:**
> I have retrieved the PDF link for CORE ID 123456. You can download the full open access version here: [URL]. Would you also like to see the article's version history?

---

**👤 You:**
> "Find information about the journal with ISSN 2041-1723."

**🤖 AI Agent:**
> The ISSN 2041-1723 corresponds to 'Nature Communications'. It is a high-profile open access journal. I can list recent articles from this journal or provide more metadata if needed.


## ❓ FAQ

**Q: How do I get the PDF of a specific research article?**
Use the `get_article_pdf` tool with the CORE Article ID. The agent will return the direct download URL for the open access PDF version of the paper.

**Q: Can I search for specific journals or repositories?**
Yes! You can use `search_journals` or `search_repositories` for general text queries, or use `get_journal` (with an ISSN) and `get_repository` (with a Repository ID) for direct lookups.

**Q: What does the OAI resolution tool do?**
The `resolve_oai` tool takes an OAI identifier (like oai:oro.open.ac.uk:75049) and resolves it to the CORE metadata page or the original repository link, helping you find the source of the research.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/core-open-access-research](https://vinkius.com/mcp/core-open-access-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CORE (Open Access Research)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `core-open-access-research` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CORE (Open Access Research)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "core-open-access-research": {
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
