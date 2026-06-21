# PubMed MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubmed)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pubmed-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pubmed-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 37M+ biomedical research articles from the world's largest medical literature database — with full abstracts, authors, MeSH terms, and citation tracking.

## Description
Connect your AI agent to the **National Library of Medicine's PubMed database** — the undisputed gold standard for biomedical and life sciences literature worldwide.

### What you can do

- **Literature Search** — Find research articles by keyword, disease name, gene symbol, drug, or any biomedical topic across 37M+ indexed articles using powerful boolean operators (AND, OR, NOT)
- **Full Article Details** — Retrieve comprehensive metadata including complete abstracts, all contributing authors, publishing journal, DOI, publication types, and MeSH descriptors for any article by PMID
- **Citation Tracking** — Discover which subsequent papers cite a specific article to trace the impact chain and follow the evolution of a research topic over time

### How it works

1. Subscribe to this server
2. Start searching PubMed from Claude, Cursor, or any MCP-compatible client — no API key required

### Who is this for?

- **Healthcare Professionals** — quickly locate clinical evidence, systematic reviews, and treatment guidelines without navigating the PubMed web interface
- **Biomedical Researchers** — run targeted literature searches and citation analyses directly from their AI coding assistant
- **Science Writers & Journalists** — find primary sources and peer-reviewed evidence for accurate scientific reporting


## Available Tools
- **get_pubmed_article**: Get full details of a PubMed article by its PMID
- **get_pubmed_citations**: Useful for tracing the impact of a paper and finding follow-up research.

Find articles that cite a specific PubMed paper
- **search_pubmed**: Returns titles, authors, journals, abstracts, DOIs, and MeSH terms. Supports boolean operators: AND, OR, NOT.

Search PubMed for biomedical and life sciences research articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubMed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find recent research on CRISPR gene therapy for sickle cell disease."

**🤖 AI Agent:**
> Found 10 recent articles on CRISPR and sickle cell disease. Highlights include: 'CRISPR-Cas9 Gene Editing for Sickle Cell Disease and β-Thalassemia' (NEJM, 2023) — a landmark clinical trial showing 97% of patients free of vaso-occlusive crises after exa-cel infusion. PMID: 38040890. Full abstract and MeSH terms retrieved.

---

**👤 You:**
> "Get complete details for PubMed article PMID 33782455."

**🤖 AI Agent:**
> Retrieved full data for PMID 33782455: 'SARS-CoV-2 variants of concern and variants of interest' by Harvey et al. Published in Nature Reviews Microbiology (2021). The abstract details the classification framework for emerging variants including Alpha, Beta, Gamma, and Delta. DOI: 10.1038/s41579-021-00573-0. MeSH Terms: COVID-19, SARS-CoV-2, Mutation, Spike Glycoprotein.

---

**👤 You:**
> "Which papers cite the original CRISPR-Cas9 paper? Show me the top citing articles."

**🤖 AI Agent:**
> Found 10 citing articles for the landmark CRISPR paper. Top citations include applications in gene therapy, agricultural biotechnology, diagnostic systems (SHERLOCK/DETECTR), and base editing. Authors span institutions from MIT, Harvard, UC Berkeley, and the Broad Institute. Each result includes PMID, DOI, and full abstract.


## Installation & Usage

To install and use the **PubMed** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubmed](https://vinkius.com/mcp/pubmed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
