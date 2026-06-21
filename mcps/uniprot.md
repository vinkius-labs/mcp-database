# UniProt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uniprot)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: What is the difference between Swiss-Prot and TrEMBL entries?**
Swiss-Prot contains 570K+ entries that have been manually reviewed and curated by expert biologists — the gold standard for protein annotation. TrEMBL contains 250M+ entries that are computationally annotated from gene sequences. Swiss-Prot entries are marked as 'reviewed' and are highly reliable; TrEMBL entries are automatically generated and may contain errors.

**Q: Do I need to register or pay for an API key?**
No. UniProt REST API is completely free and open without any authentication. There are no rate limits for reasonable usage patterns. UniProt is funded by the National Institutes of Health (NIH), European Molecular Biology Laboratory (EMBL), and the Swiss Institute of Bioinformatics (SIB).

**Q: Can I retrieve full amino acid sequences for proteins?**
Yes. Every protein entry includes the full amino acid sequence with length information. The sequence is returned in standard one-letter amino acid code. For very large proteins (10,000+ residues), the sequence may be truncated in the response but the full accession data is always provided for direct download.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniprot](https://vinkius.com/mcp/uniprot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UniProt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uniprot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UniProt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uniprot": {
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
