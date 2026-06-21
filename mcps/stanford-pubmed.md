# Stanford PubMed MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stanford-pubmed)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stanford-pubmed-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stanford-pubmed-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Search biomedical literature from the world largest database of life science and medical research publications.

## Description
Connect to the **PubMed E-utilities API** from the National Library of Medicine — the gold standard for biomedical literature search.

### What you can do

- **Full-Text Search** — Search across 36M+ biomedical articles from MEDLINE
- **MeSH Vocabulary** — Use Medical Subject Headings for precise, controlled-vocabulary searches
- **Clinical Trials** — Filter specifically for clinical trial publications
- **Reviews & Meta-analyses** — Find systematic reviews and meta-analyses
- **Gene Search** — Search articles mentioning specific genes (TP53, BRCA1, EGFR)
- **Drug Search** — Find articles about specific drugs and compounds
- **Citation Tracking** — Find articles that cite a given paper
- **Related Articles** — Use NCBI's similarity algorithm to discover related literature
- **Abstracts** — Retrieve full structured abstracts for quick evaluation
- **Free Full Text** — Filter for open access articles available in PubMed Central
- **Batch Retrieval** — Fetch multiple articles by PMID in a single request

### Who is this for?

- **Medical Researchers** — literature reviews, evidence-based medicine
- **PhD Students** — comprehensive biomedical search
- **Clinicians** — find clinical trial evidence for treatment decisions
- **Pharmacologists** — drug interaction and efficacy research


## Available Tools
- **batch_get_articles**: Useful for building reading lists, comparing studies, or analyzing a collection of articles from a reference list.

Retrieve multiple articles by PMID list
- **get_abstract**: For structured abstracts, returns all sections (Background, Methods, Results, Conclusions). Essential for quickly evaluating whether a paper is relevant without accessing the full text.

Get the full abstract text of a PubMed article
- **get_article**: Returns title, all authors, journal name, publication date, volume, issue, pages, DOI, publication types, and language.

Get article details by PubMed ID (PMID)
- **get_citations**: Essential for understanding an article's impact, finding follow-up studies, and tracking how findings have been built upon by other researchers.

Get articles that cite a given PubMed article
- **get_related_articles**: The algorithm considers title, abstract, MeSH headings, and substances to compute similarity scores. This is often more effective than keyword search for discovering relevant literature.

Find related articles using NCBI similarity algorithm
- **search_by_author**: Use "LastName FirstInitial" format for best results (e.g. "Doudna JA", "Zhang F"). Returns the author's publication list with article metadata.

Find PubMed articles by author name
- **search_by_journal**: Can be combined with a topic query. Use journal abbreviations or full names (e.g. "Nature", "N Engl J Med", "Lancet", "Cell", "Science", "JAMA", "BMJ").

Find articles published in a specific journal
- **search_by_mesh**: MeSH terms provide precise topic classification. Examples: "Neoplasms", "Diabetes Mellitus", "Machine Learning", "Clustered Regularly Interspaced Short Palindromic Repeats", "COVID-19".

Search using MeSH controlled vocabulary terms
- **search_clinical**: This includes Phase I-IV trials, randomized controlled trials, and clinical study reports. Essential for evidence-based medicine and systematic reviews.

Search for clinical trial publications
- **search_drugs**: Uses the Substance Name field for precise matching. Examples: "metformin", "pembrolizumab", "remdesivir", "aspirin", "dexamethasone".

Search articles mentioning specific drugs or compounds
- **search_free_full_text**: This filters to only return open access or author-deposited articles where the complete manuscript can be read for free. Essential for researchers without institutional journal subscriptions.

Search for articles with free full-text available
- **search_genes**: Uses the Gene Name field tag for precise matching. Examples: "TP53", "BRCA1", "EGFR", "KRAS", "MYC". Can be combined with a topic query for more specific results.

Search articles mentioning specific genes
- **search_pubmed**: Returns article titles, authors, journals, dates, DOIs, and publication types. Sort options: "relevance" (default), "date", "pub_date", "first_author", "journal".

Search 36M+ biomedical articles on PubMed
- **search_recent**: Use this to stay up-to-date with the latest publications in your research area. Default is last 30 days.

Find the most recent articles in a field
- **search_reviews**: These are the highest level of evidence synthesis in medicine and provide comprehensive overviews of research on a topic.

Search for review articles and meta-analyses
- **search_trending**: This surfaces papers that are generating the most attention and engagement in the research community.

Find trending articles in a subject area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stanford PubMed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find recent clinical trials for CAR-T cell therapy in lymphoma"

**🤖 AI Agent:**
> I've searched PubMed for clinical trial publications on "CAR-T cell therapy lymphoma". The results include recent Phase I-III trials from major cancer centers.

---

**👤 You:**
> "Search for BRCA1 gene articles related to breast cancer prevention"

**🤖 AI Agent:**
> I've found PubMed articles mentioning the BRCA1 gene in the context of breast cancer prevention, including studies on genetic screening and prophylactic interventions.

---

**👤 You:**
> "Find free full-text systematic reviews on metformin and diabetes prevention"

**🤖 AI Agent:**
> I've filtered PubMed for free full-text systematic reviews on metformin and diabetes prevention, returning open-access meta-analyses from PubMed Central.


## Installation & Usage

To install and use the **Stanford PubMed** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stanford-pubmed](https://vinkius.com/mcp/stanford-pubmed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
