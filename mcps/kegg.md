# KEGG MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kegg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kegg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kegg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the Kyoto Encyclopedia of Genes and Genomes (KEGG) to query genomic, chemical, and systemic functional information directly from your AI agent.

## Description
Connect your AI agent to the **KEGG** (Kyoto Encyclopedia of Genes and Genomes) database, the gold standard for bioinformatics and systems biology. This server enables deep exploration of biological pathways, genomes, and chemical substances through natural language.

### What you can do

- **Genomic Exploration** — Retrieve detailed information about genes, proteins, and organisms using `kegg_get` and `kegg_list`.
- **Pathway Analysis** — Map genes to metabolic or signaling pathways and visualize biological systems using `kegg_link`.
- **Chemical & Drug Data** — Search for compounds, glycans, and drugs by keyword, formula, or mass using `kegg_find`.
- **Drug Interactions** — Identify adverse drug-drug interactions (DDI) specifically for clinical and pharmacological research via `kegg_ddi`.
- **Identifier Conversion** — Seamlessly convert between KEGG IDs and outside databases like NCBI, UniProt, and PubChem using `kegg_conv`.

### How it works

1. Subscribe to this server
2. Configure your access credentials (if required by your proxy)
3. Start querying biological data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bioinformatics Researchers** — automate the retrieval of gene sequences and pathway maps without manual REST calls.
- **Pharmacologists** — quickly check drug-drug interactions and chemical properties during drug discovery workflows.
- **Data Scientists** — integrate high-quality biological metadata into analysis pipelines directly from the chat interface.


## Available Tools
- **kegg_conv**: Converts KEGG identifiers to/from outside identifiers
- **kegg_ddi**: Finds adverse drug-drug interactions
- **kegg_find**: Finds entries matching a query keyword or chemical data
- **kegg_get**: g., hsa:10458+ece:Z5100).

Retrieves database entries in flat-file or specific file formats
- **kegg_info**: g., kegg, pathway, brite, genes, hsa, compound).

Displays database release information and statistics
- **kegg_link**: g., pathways linked from human genes).

Finds related entries using database cross-references
- **kegg_list**: For pathway/brite, can specify organism/option. Use "organism" to list all KEGG organisms.

Obtains a list of entry identifiers and associated names


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KEGG** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available organisms in the KEGG database."

**🤖 AI Agent:**
> I'll use `kegg_list` with the 'organism' parameter. I've found thousands of entries, including 'hsa' (Homo sapiens), 'mmu' (Mus musculus), and 'eco' (Escherichia coli). Which one would you like to explore?

---

**👤 You:**
> "Search for compounds with the keyword 'glucose' in the KEGG database."

**🤖 AI Agent:**
> Running `kegg_find` for 'glucose' in the compound database... I found several entries, including C00031 (D-Glucose) and C00221 (beta-D-Glucose). Would you like the full details for C00031?

---

**👤 You:**
> "Get the full entry details for the human gene hsa:10458."

**🤖 AI Agent:**
> Fetching data using `kegg_get` for 'hsa:10458'... This gene corresponds to ACSL4 (acyl-CoA synthetase long chain family member 4). It is involved in metabolic pathways like Fatty acid metabolism (hsa00071).


## Installation & Usage

To install and use the **KEGG** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kegg](https://vinkius.com/mcp/kegg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
