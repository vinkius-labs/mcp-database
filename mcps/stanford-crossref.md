# Stanford CrossRef MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-crossref)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stanford-crossref-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stanford-crossref-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Query scholarly metadata for millions of academic publications with DOI resolution, citation tracking, and publisher data.

## Description
Connect to the **CrossRef API** — the authoritative source for DOI metadata and scholarly publishing infrastructure.

### What you can do

- **DOI Resolution** — Resolve any DOI to complete bibliographic metadata
- **Works Search** — Search 150M+ DOI-registered works with advanced filters
- **Journal Registry** — Query journals by title or ISSN with coverage metrics
- **Publisher Profiles** — Explore academic publishers (Elsevier, Springer, Wiley)
- **Funder Registry** — Search funding organizations (NIH, NSF, ERC, Wellcome Trust)
- **ORCID Lookup** — Find works by researcher ORCID identifier
- **Affiliation Search** — Search works by institutional affiliation
- **Citation Counts** — Get citation and reference counts for any DOI
- **Reference Lists** — Extract complete bibliographies from published works
- **Preprint Search** — Find preprints registered with CrossRef
- **DOI Validation** — Verify whether a DOI is valid and registered
- **Recent Works** — Monitor the latest DOI registrations

### Who is this for?

- **Researchers** — DOI resolution and bibliography management
- **Librarians** — journal evaluation and publisher analysis
- **Research Administrators** — funder tracking and institutional output
- **Bibliometricians** — large-scale publication analytics


## Available Tools
- **get_citations_count**: The "is-referenced-by-count" is the number of times other works cite this DOI. The "references-count" is how many references this work cites. Quick way to assess a paper's impact.

Get citation count for a DOI
- **get_funder_works**: Use the funder ID from search_funders (e.g. "100000002" for NIH). Essential for understanding research funding landscapes and tracking funded output.

Get works funded by a specific funding organization
- **get_journal**: Returns title, publisher, subjects, total DOI count, current and backfile counts, metadata coverage percentages, and quality flags.

Get journal details by ISSN
- **get_journal_works**: Can be filtered with an optional text query. Useful for browsing a journal's publication history or searching within a specific journal.

Get articles published in a specific journal
- **get_publisher**: Returns name, DOI prefix, total/current/backfile DOI counts, metadata coverage scores, and quality flags.

Get publisher details with output metrics
- **get_reference_list**: Returns all cited references with their DOIs (when available), authors, titles, journals, and years. Essential for bibliography analysis, finding source material, and understanding a paper's intellectual foundations.

Get full reference list (bibliography) for a DOI
- **resolve_doi**: Returns title, authors, journal, publisher, publication date, volume, issue, pages, citation count, reference count, subject areas, and license information. The definitive tool for getting structured metadata from any DOI.

Resolve a DOI to full bibliographic metadata
- **search_by_affiliation**: Use institution names like "Stanford University", "MIT", "Harvard Medical School". Can be combined with a topic query.

Search works by institutional affiliation
- **search_by_orcid**: ORCID is the universal researcher identifier. Format: "0000-0002-1825-0097". Essential for finding the complete publication record of a researcher across all journals and publishers.

Find works by ORCID author identifier
- **search_funders**: Examples: "National Institutes of Health", "National Science Foundation", "European Research Council", "Wellcome Trust".

Search funding organizations worldwide
- **search_journals**: Returns journal titles, ISSNs, publishers, subject areas, total DOI counts, and metadata coverage scores. Use this to find journal identifiers and evaluate journal metrics.

Search academic journals by title or ISSN
- **search_preprints**: This covers preprints from bioRxiv, medRxiv, SSRN, ChemRxiv, and other preprint servers that register DOIs with CrossRef.

Search registered preprints across all servers
- **search_publishers**: Returns publisher names, DOI prefixes, and total DOI counts.

Search academic publishers
- **search_recent_works**: Default is last 7 days. Use this to monitor the latest publications across all journals and publishers.

Find the most recently registered DOIs
- **search_works**: Supports full-text query, filters, sorting, and pagination. Filter syntax: "from-pub-date:2024-01-01", "type:journal-article", "has-orcid:true", "has-references:true", "is-update:false". Sort options: "relevance", "published", "indexed", "is-referenced-by-count".

Search 150M+ DOI-registered academic works
- **validate_doi**: Returns whether the DOI exists in CrossRef, along with basic metadata (title, type, publisher) if valid. Useful for quality-checking reference lists and citation data.

Check if a DOI is valid and registered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stanford CrossRef** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve DOI 10.1038/s41586-021-03819-2"

**🤖 AI Agent:**
> I've resolved this DOI via CrossRef. It is: "Highly accurate protein structure prediction with AlphaFold" by Jumper et al., published in Nature (2021). It has been cited over 15,000 times.

---

**👤 You:**
> "Find works funded by the National Institutes of Health on gene therapy"

**🤖 AI Agent:**
> I've searched for NIH-funded works on gene therapy via CrossRef. Results include recent publications in Nature Medicine, Science, and Cell acknowledging NIH grants.

---

**👤 You:**
> "Look up all publications by ORCID 0000-0002-8350-519X"

**🤖 AI Agent:**
> I've retrieved all DOI-registered works for this ORCID via CrossRef, showing titles, journals, publication dates, and citation counts for each.


## Installation & Usage

To install and use the **Stanford CrossRef** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-crossref](https://vinkius.com/mcp/stanford-crossref)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
