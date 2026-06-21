# Stanford Semantic Scholar MCP Server

Discover academic papers with AI-powered search that understands research context, finds citations, and recommends related work.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-semantic-scholar)

## Overview
**Category:** education
**Tools Count:** 16

## Description
Connect to the **Semantic Scholar Academic Graph API** and unlock the world's largest free academic knowledge graph.

### What you can do

- **Paper Search** — Full-text search across 200M+ papers with filters for year, field of study, venue, and open access
- **Citation Analysis** — Navigate forward citations (who cited this?) and backward references (what did this cite?)
- **Author Profiles** — Search and retrieve author metrics including h-index, paper count, and citation count
- **Batch Operations** — Retrieve multiple papers or authors in a single request for efficient analysis
- **AI Recommendations** — Get machine learning-powered paper recommendations from single or multiple seed papers
- **Venue Filtering** — Search within specific conferences (NeurIPS, ICML, CVPR) or journals (Nature, Science, Cell)
- **Field Filtering** — Search within specific fields: Computer Science, Medicine, Biology, Physics, and 20+ more

### How it works

1. Subscribe to this server
2. No API key required — the API is fully public
3. Start searching papers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — conduct literature reviews, find related work, discover citation chains
- **PhD Students** — navigate the academic graph to position your research
- **Data Scientists** — build publication analytics and bibliometric analyses
- **R&D Teams** — monitor the latest publications in your domain


## Available Tools
- **batch_get_authors**: Returns names, affiliations, paper counts, citation counts, and h-indices. Useful for comparing researchers or building collaboration network analyses.

Retrieve multiple author profiles in a single request
- **batch_get_papers**: Accepts S2 IDs, DOIs, ArXiv IDs, or PubMed IDs. Useful for comparing papers, building reading lists, or analyzing a set of related works.

Retrieve multiple papers in a single request
- **bulk_search_papers**: Each call returns a batch of results plus a continuation token. Pass the token in subsequent calls to get the next batch. Ideal for systematic literature reviews and meta-analyses.

Bulk search for large result sets with token pagination
- **get_author**: Returns name, affiliations, homepage, external IDs (DBLP, ORCID), total paper count, citation count, and h-index. The definitive tool for understanding a researcher's academic impact.

Get author profile with h-index, citations, and metrics
- **get_author_papers**: Returns papers with titles, years, venues, citation counts, open access status, and fields of study. Essential for reviewing a researcher's body of work or finding specific publications by a known author.

Get all papers by a specific author
- **get_multi_recommendations**: The algorithm finds papers similar to the positive set but dissimilar to the negative set. Ideal for focused literature discovery.

Get recommendations from multiple seed papers with positive/negative signals
- **get_paper**: Accepts multiple ID formats: Semantic Scholar ID (e.g. "649def34f8be52c8b66281af98ae884c09aef38b"), DOI (e.g. "10.1038/s41586-021-03819-2"), ArXiv ID (e.g. "arXiv:2106.09685"), PubMed ID (e.g. "PMID:34845388"), or ACL ID (e.g. "ACL:W12-3903"). Returns title, abstract, authors, venue, year, citation counts, open access PDF URL, and publication metadata.

Get full paper details by ID, DOI, ArXiv ID, or PubMed ID
- **get_paper_authors**: Useful for identifying research leaders and collaboration networks.

Get authors of a specific paper with h-index and metrics
- **get_paper_citations**: This is essential for understanding a paper's impact, finding follow-up work, and tracing how an idea has evolved. Returns citing paper metadata including titles, venues, years, and citation counts.

Get papers that cite a given paper
- **get_paper_references**: Essential for literature reviews, understanding the intellectual lineage of a work, and finding foundational papers in a research area.

Get papers referenced by a given paper
- **get_recommendations**: The algorithm analyzes citation patterns, co-citation networks, and content similarity to find the most relevant papers you should read next. This is the AI-native way to discover related literature.

Get AI-powered paper recommendations from a seed paper
- **match_paper_title**: Uses fuzzy matching to handle slight variations. Returns the best matching paper with a match score. Ideal when you have a paper title from a reference list or bibliography and need to find its full metadata.

Find an exact paper match from a title string
- **search_authors**: Returns author profiles with affiliations, paper counts, citation counts, and h-index. Use this to find researchers in a specific field, discover top contributors, or find collaborators.

Search authors by name across the academic graph
- **search_by_field**: Supported fields: Computer Science, Medicine, Biology, Chemistry, Physics, Mathematics, Engineering, Environmental Science, Economics, Business, Political Science, Sociology, Psychology, Art, History, Geography, Philosophy, Materials Science, Geology, Linguistics, Education, Agricultural and Food Sciences, Law.

Search papers filtered by field of study
- **search_by_venue**: Use venue names like "Nature", "Science", "NeurIPS", "ICML", "CVPR", "ACL", "EMNLP", "The Lancet", "JAMA", "Cell", "Physical Review Letters". Essential for tracking publications in specific top-tier venues.

Search papers filtered by conference or journal
- **search_papers**: Returns titles, venues, years, citation counts, open access status, fields of study, and authors. Supports filtering by year range (e.g. "2020-2024"), fields of study (e.g. "Computer Science"), venue (e.g. "Nature"), and open access availability.

Search across 200M+ academic papers by keyword


## Installation & Usage

To install and use the **Stanford Semantic Scholar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-semantic-scholar](https://vinkius.com/mcp/stanford-semantic-scholar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
