# CrossRef MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crossref-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 150M+ academic works — find journal articles, books, DOIs, citations and scholarly metadata.

## Description
Connect to **CrossRef** and explore the world's largest scholarly metadata database through natural conversation — no API key needed.

### What you can do

- **Work Search** — Search 150M+ academic works by title, author, DOI, keywords or abstract
- **DOI Lookup** — Get complete metadata for any academic work by its DOI
- **Journal Search** — Browse academic journals by name with ISSNs and work counts
- **Publisher Search** — Find academic publishers with their work counts and journal lists
- **Funder Search** — Discover research funding organizations and their funded works
- **Member Search** — Browse CrossRef member organizations that register DOIs
- **Work Types** — Explore publication types (journal-article, book-chapter, proceedings, dataset)
- **Licenses** — View academic licenses used in scholarly works

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore academic metadata from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — find relevant papers, check citation counts and discover related works
- **Students** — search for papers by topic, find journals and explore academic literature
- **Librarians** — look up DOIs, verify citations and discover journal metadata


## Available Tools (13)
- **get_funder**: Returns funder name, country, URI, work count and location info.

Get details for a specific research funder
- **get_journal**: Returns journal title, ISSNs, publisher, work count and URL.

Get details for a specific journal by ISSN
- **get_licenses**: Returns license IDs, URLs and names.

Get list of known licenses used in academic works
- **get_member**: Returns member name, prefixes, work counts and location info.

Get details for a specific CrossRef member
- **get_publisher**: Returns publisher name, work count, journal count and location info.

Get details for a specific publisher
- **get_types**: ). Useful for filtering searches by publication type.

Get list of academic work types
- **get_work**: Returns title, authors, abstract, publication date, journal, publisher, license, references, citation count and full citation info.

Get metadata for a specific academic work by DOI
- **get_works_by_doi_list**: Provide a comma-separated list of DOIs. Returns metadata for each work including title, authors, publication date and journal.

Get metadata for multiple works by their DOIs
- **search_funders**: Returns funder names, IDs, country codes, URIs and work counts.

Search research funders by name
- **search_journals**: Returns journal titles, ISSNs, publisher names and work counts.

Search academic journals by name
- **search_members**: Returns member names, IDs, prefixes and work counts.

Search CrossRef member organizations
- **search_publishers**: Returns publisher names, work counts, journal counts and organization names.

Search academic publishers by name
- **search_works**: Supports free-text query and advanced filtering by type, publication date, author, journal, publisher, funder, license and more. Returns titles, authors, publication dates, DOIs, citation counts and abstracts.

Search academic works by title, author, DOI or keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrossRef** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for papers about machine learning published in 2024."

**🤖 AI Agent:**
> Found 50+ papers about machine learning from 2024. Top results include works in Nature Machine Intelligence, IEEE Transactions, ACM Computing Surveys. Each with DOIs, authors, abstracts and citation counts.

---

**👤 You:**
> "Get metadata for DOI 10.1038/nature12373."

**🤖 AI Agent:**
> Title: 'Deep learning in neural networks: An overview'. Authors: Jürgen Schmidhuber. Journal: Neural Networks, 2015. Publisher: Elsevier. Citations: 15,000+. DOI: 10.1016/j.neunet.2014.09.003.

---

**👤 You:**
> "Find journals published by Nature Publishing Group."

**🤖 AI Agent:**
> Found 100+ journals from Springer Nature including: Nature (ISSN: 0028-0836, 200K+ works), Nature Medicine, Nature Biotechnology, Nature Communications, Scientific Reports. Each with ISSN, work counts and URLs.


## ❓ FAQ

**Q: Do I need an API key?**
No! CrossRef API is completely free and open. No authentication required. Just subscribe and start searching. Rate limit is 50 requests/second for polite pool.

**Q: What is a DOI?**
DOI (Digital Object Identifier) is a unique alphanumeric string assigned to academic works. It provides a persistent link to the work's location online. Example: 10.1038/nature12373.

**Q: How can I filter search results?**
Use the filter parameter with CrossRef filter syntax. Examples: 'type:journal-article' for journal articles only, 'from-pub-date:2024' for papers from 2024 onwards, 'has-abstract:true' for papers with abstracts, 'has-full-text:true' for open access papers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crossref-alternative](https://vinkius.com/mcp/crossref-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrossRef** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crossref-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrossRef** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crossref-alternative": {
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
