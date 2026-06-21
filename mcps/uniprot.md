# UniProt MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uniprot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uniprot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uniprot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 250M+ protein sequences with functional annotations, gene names, subcellular locations, and amino acid data from the world's most comprehensive protein knowledge base.

## Description
Connect your AI agent to **UniProt** — the Universal Protein Resource — the world's definitive knowledge base for protein sequence and functional information.

### What you can do

- **Protein Search** — Find proteins by name, gene symbol, function, or organism across 250M+ entries from both TrEMBL (auto-annotated) and Swiss-Prot (manually curated)
- **Accession Lookup** — Get complete protein data by UniProt accession number (e.g., P04637 for human p53) including function, subcellular location, and full amino acid sequence
- **Gene Search** — Find all proteins encoded by a specific gene name across multiple organisms to compare orthologs and paralogs

### How it works

1. Subscribe to this server
2. Start searching proteins immediately — no API key required

### Who is this for?

- **Molecular Biologists** — quickly look up protein functions, domains, and post-translational modifications for experimental design
- **Bioinformaticians** — retrieve protein sequences and annotations programmatically for large-scale comparative analyses
- **Drug Discovery Teams** — identify therapeutic targets by searching protein functions and disease associations


## Available Tools
- **get_uniprot_protein**: Get full protein details by UniProt accession ID
- **search_uniprot_gene**: Returns all protein isoforms and their functional annotations.

Find proteins encoded by a specific gene
- **search_uniprot**: Returns protein name, gene, organism, function, subcellular location, and sequence. Try: insulin, hemoglobin, p53, BRCA1, spike protein.

Search UniProt for proteins by name, function, or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UniProt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me about the p53 tumor suppressor protein and its function."

**🤖 AI Agent:**
> P53_HUMAN (UniProt P04637): Gene TP53, Homo sapiens. 393 amino acids. Swiss-Prot reviewed ✅. Function: Acts as a tumor suppressor in many tumor types by inducing growth arrest or apoptosis. Activated in response to DNA damage, oncogene activation, and hypoxia. Located in nucleus and cytoplasm. Critical note: TP53 is the most frequently mutated gene in human cancers.

---

**👤 You:**
> "Find all proteins encoded by the BRCA1 gene."

**🤖 AI Agent:**
> Found 10 entries for gene BRCA1. Top result: BRCA1_HUMAN (P38398, Swiss-Prot reviewed ✅) — Homo sapiens, 1863 amino acids. Function: E3 ubiquitin ligase, key role in DNA repair via homologous recombination. Mutations associated with increased risk of breast and ovarian cancer. Also found orthologs in mouse (Q61187), rat, and zebrafish.

---

**👤 You:**
> "Look up UniProt accession Q9BYF1 and show me its full details."

**🤖 AI Agent:**
> Q9BYF1: ACE2_HUMAN — Angiotensin-converting enzyme 2. Gene: ACE2, Homo sapiens. 805 amino acids. Swiss-Prot reviewed ✅. Function: Metalloprotease that converts angiotensin II to angiotensin-(1-7). Notably serves as the functional receptor for SARS-CoV and SARS-CoV-2 spike proteins. Located in cell membrane.


## Installation & Usage

To install and use the **UniProt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniprot](https://vinkius.com/mcp/uniprot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
