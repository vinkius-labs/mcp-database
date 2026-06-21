# Stanford OpenAlex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-openalex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Explore the global research landscape with open access to scholarly works, authors, institutions, and citation graphs.

## Description
Connect to the **OpenAlex API** — the fully open catalog of the global research system.

### What you can do

- **Works** — Search and analyze 250M+ academic works (papers, books, datasets, patents)
- **Authors** — Browse 90M+ researcher profiles with h-index, i10-index, and citation metrics
- **Institutions** — Explore 100K+ universities, labs, and research organizations worldwide
- **Sources** — Query 240K+ journals, conferences, and repositories with impact metrics
- **Concepts** — Navigate the 65K+ scientific concept taxonomy from broad to specific
- **Funders** — Discover which organizations fund specific research areas
- **Publishers** — Analyze the academic publishing landscape
- **Topics** — Explore hierarchical topic classifications across all of science
- **Open Access** — Find freely available research papers

### How it works

1. Subscribe to this server
2. No API key required — OpenAlex is 100% free and open
3. Start exploring the academic world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Research Administrators** — benchmark institutions, track funding landscapes
- **Bibliometricians** — analyze publication trends, citation patterns, and research impact
- **Science Policy Makers** — understand research funding and output by country and institution
- **Academic Librarians** — explore journal metrics and open access availability


## Available Tools (16)
- **get_author**: Returns name, affiliations, paper count, citation count, h-index, i10-index, 2-year mean citedness, top research concepts, and publication trends by year. The definitive tool for assessing academic impact.

Get author profile with h-index, citations, and impact metrics
- **get_author_works**: Returns works with titles, DOIs, years, citation counts, open access status, and primary venues. Sort by "cited_by_count:desc" for most cited or "publication_date:desc" for most recent.

Get all works by a specific author
- **get_concept**: Essential for understanding the structure of a research field.

Get concept details with ancestors, related concepts, and trends
- **get_funder**: Use this to understand which organizations fund specific research areas.

Get funder details and funded research statistics
- **get_institution**: Get institution details with research metrics and collaborations
- **get_source**: Essential for evaluating journal quality and coverage.

Get journal or conference details with impact metrics
- **get_work**: Accepts OpenAlex IDs (e.g. "W2741809807"), DOIs (e.g. "https://doi.org/10.1038/s41586-021-03819-2"), PubMed IDs (e.g. "pmid:34845388"), or MAG IDs. Returns title, abstract, authors with institutions, concepts, citation count, open access status, and publication details.

Get academic work details by OpenAlex ID, DOI, or PubMed ID
- **search_authors**: Returns display name, ORCID, works count, citation count, h-index, i10-index, and last known institution. Filter examples: "cited_by_count:>10000", "works_count:>100", "last_known_institutions.country_code:US".

Search 90M+ academic authors by name
- **search_concepts**: Returns names, levels, descriptions, works counts, and citation counts.

Search 65K+ scientific concepts in the knowledge hierarchy
- **search_funders**: Returns names, countries, grants counts, works funded, and citation impact. Essential for understanding research funding landscapes.

Search funding organizations worldwide
- **search_institutions**: Returns names, countries, types, works counts, citation counts, and homepages. Filter examples: "country_code:US", "type:education", "cited_by_count:>1000000".

Search 100K+ research institutions worldwide
- **search_open_access**: This is a specialized filter of the works endpoint that returns only papers with open access PDFs. Ideal for researchers who need freely accessible literature for reading, citation, or meta-analysis.

Search only open access academic works
- **search_publishers**: Returns names, countries, works counts, and citation counts. Useful for analyzing the publishing landscape.

Search academic publishers
- **search_sources**: Returns names, ISSNs, types, works counts, citation counts, and open access status. Filter examples: "type:journal", "is_oa:true", "cited_by_count:>100000".

Search 240K+ academic journals, conferences, and repositories
- **search_topics**: Returns topic names, descriptions, associated works and citations, plus the parent field and domain. Use this to map the landscape of a research area.

Search topic classifications across all of science
- **search_works**: Supports full-text search plus structured filters. Filter syntax examples: "publication_year:2024", "open_access.is_oa:true", "type:journal-article", "cited_by_count:>100". Sort options: "cited_by_count:desc", "publication_date:desc", "relevance_score:desc".

Search 250M+ academic works by keyword or filter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stanford OpenAlex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which universities have the highest research output in AI?"

**🤖 AI Agent:**
> I've searched OpenAlex for institutions with the highest works count in artificial intelligence concepts. The top institutions include MIT, Stanford University, Carnegie Mellon, UC Berkeley, and Tsinghua University.

---

**👤 You:**
> "What are the most cited open access papers on CRISPR?"

**🤖 AI Agent:**
> I've found the most cited open access papers on CRISPR from OpenAlex, sorted by citation count. The foundational papers by Doudna and Charpentier lead the list.

---

**👤 You:**
> "Show me the concept hierarchy for machine learning"

**🤖 AI Agent:**
> I've retrieved the Machine Learning concept from OpenAlex. It sits at level 1 under Computer Science (level 0), and has child concepts including Deep Learning, Neural Networks, Reinforcement Learning, and Natural Language Processing at finer granularity levels.


## ❓ FAQ

**Q: Do I need an API key?**
No. OpenAlex is 100% free and open. No registration or API key is required.

**Q: How is OpenAlex different from Semantic Scholar?**
OpenAlex provides a broader ecosystem view with entities for institutions, journals, funders, publishers, and concepts — not just papers and authors. It is ideal for bibliometric analysis, institutional benchmarking, and understanding the structure of the research system. Semantic Scholar excels at AI-powered recommendations and citation graph navigation.

**Q: What replaced Microsoft Academic Graph?**
OpenAlex was created as the free, open-source successor to Microsoft Academic Graph (MAG), which was discontinued in 2022. OpenAlex now contains over 250 million works and continues to grow, fully funded by grants to ensure permanent public access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-openalex](https://vinkius.com/mcp/stanford-openalex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stanford OpenAlex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stanford-openalex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stanford OpenAlex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stanford-openalex": {
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
