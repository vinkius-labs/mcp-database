# PubMed Central MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubmed-central)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and retrieve full-text biomedical and life sciences literature from PubMed Central (PMC).

## Description
Connect your AI agent to **PubMed Central (PMC)**, the world's premier digital archive of biomedical and life sciences journal literature. This server enables deep exploration of millions of open-access articles directly through natural conversation.

### What you can do

- **Advanced Search** — Use `search_articles` to find PMCIDs matching complex queries, including authors, dates, and specific filters.
- **Full-Text Retrieval** — Access complete article content in BioC XML or JSON formats using `get_bioc_article` for deep analysis.
- **Citation Analysis** — Track the scientific impact of research by finding articles that cite a specific PMID with `get_citing_articles`.
- **Identifier Mapping** — Seamlessly convert between PMCIDs, PMIDs, and DOIs using `convert_ids` to ensure data consistency.
- **Metadata Harvesting** — Retrieve document summaries, license information, and file locations for Open Access records via `get_article_summary` and `get_oa_record`.

### How it works

1. Subscribe to this server
2. Provide your NCBI Tool Name and Email (and an optional API Key for higher rate limits)
3. Start querying the global repository of medical knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — Instantly find relevant literature and extract data from full-text papers without manual downloading.
- **Healthcare Professionals** — Quickly verify medical facts and access the latest clinical studies directly from your workspace.
- **Data Scientists** — Automate the collection of biomedical datasets and citation networks for large-scale analysis.


## Available Tools
- **get_bioc_article**: Retrieve full-text articles via the BioC API
- **get_citing_articles**: Find PMC articles that cite a specific PubMed ID
- **convert_ids**: Convert between article identifiers (PMCID, PMID, DOI)
- **get_oa_record**: Find citation data, license info, and file locations for OA articles
- **oai_pmh_request**: Harvest metadata via the PMC OAI-PMH Service
- **search_articles**: Search for articles in PubMed Central
- **get_article_summary**: Get metadata summaries for PMC articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubMed Central** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search PubMed Central for recent articles about 'CRISPR gene editing' published in 2023."

**🤖 AI Agent:**
> I found several articles. Notable ones include PMC1012345 ('Advances in CRISPR...') and PMC1023456. Would you like a summary of the most relevant one?

---

**👤 You:**
> "Get the full-text content of article PMC7840891 in JSON format."

**🤖 AI Agent:**
> I've retrieved the BioC JSON for PMC7840891. It contains sections for Introduction, Methods, Results, and Discussion. Which part should I analyze first?

---

**👤 You:**
> "Convert the DOI 10.1038/s41586-020-2012-7 to a PMCID."

**🤖 AI Agent:**
> The DOI 10.1038/s41586-020-2012-7 maps to PMCID: PMC7095063 (and PMID: 32015508).


## ❓ FAQ

**Q: How do I convert a DOI or PMID into a PMCID for full-text access?**
Use the `convert_ids` tool. Provide a comma-separated list of identifiers, and the agent will return the mapped PMCID, which is required for many other PMC retrieval tools.

**Q: Can I retrieve the actual content of an article, not just the abstract?**
Yes. If the article is in the Open Access subset, use `get_bioc_article` with the PMCID. You can specify 'json' or 'xml' format to get the full-text sections.

**Q: How can I find which papers have cited a specific study?**
Use the `get_citing_articles` tool by providing the PubMed ID (PMID) of the study. It will return a list of PMC articles that reference that specific work.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubmed-central](https://vinkius.com/mcp/pubmed-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PubMed Central** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pubmed-central` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PubMed Central** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pubmed-central": {
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
