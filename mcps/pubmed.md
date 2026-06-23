# PubMed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubmed)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: Do I need an API key or any registration to use PubMed?**
No. PubMed E-utilities are freely accessible to everyone without registration. An optional API key (available at ncbi.nlm.nih.gov) increases your rate limit from 3 to 10 requests per second, but is not required for standard usage.

**Q: What types of searches are supported and how can I refine my results?**
You can search by keyword, disease name, gene symbol, drug name, author surname, or journal title. Boolean operators (AND, OR, NOT) and field tags like [Title], [Author], and [MeSH Terms] work natively. Example: 'CRISPR AND cancer NOT review' targets original research on CRISPR in oncology.

**Q: Can I access full-text articles through this server?**
This server returns complete abstracts and metadata for all indexed articles. Full-text access depends on publisher open access policies — articles from PubMed Central (PMC) are freely available. The DOI link provided with each result allows direct navigation to the publisher's page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubmed](https://vinkius.com/mcp/pubmed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PubMed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pubmed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PubMed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pubmed": {
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
