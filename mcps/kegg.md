# KEGG MCP Server

Access the Kyoto Encyclopedia of Genes and Genomes (KEGG) to query genomic, chemical, and systemic functional information directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kegg)

## Overview
**Category:** databases
**Tools Count:** 7

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


## Installation & Usage

To install and use the **KEGG** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kegg](https://vinkius.com/mcp/kegg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
