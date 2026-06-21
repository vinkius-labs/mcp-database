# Stanford CrossRef MCP Server

Query scholarly metadata for millions of academic publications with DOI resolution, citation tracking, and publisher data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-crossref)

## Overview
**Category:** education
**Tools Count:** 16

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


## Installation & Usage

To install and use the **Stanford CrossRef** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-crossref](https://vinkius.com/mcp/stanford-crossref)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
