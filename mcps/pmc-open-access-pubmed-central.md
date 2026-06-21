# PMC Open Access (PubMed Central) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pmc-open-access-pubmed-central)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pmc-open-access-pubmed-central-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pmc-open-access-pubmed-central-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of open-access biomedical and life sciences research articles. Search metadata, convert IDs, and discover full-text resources.

## Description
Connect to the **PubMed Central (PMC) Open Access Subset** to empower your AI agent with direct access to millions of peer-reviewed biomedical research articles. This server provides comprehensive tools for literature discovery, metadata harvesting, and identifier management.

### What you can do

- **Metadata Harvesting** — Use OAI-PMH protocols to list identifiers, metadata formats, and full records from the PMC repository.
- **Identifier Conversion** — Seamlessly translate between PMCIDs, PMIDs, DOIs, and Manuscript IDs using the official PMC ID Converter.
- **Resource Discovery** — Locate downloadable PDF, XML, and TGZ files for open-access articles to facilitate deep analysis.
- **Citation Export** — Retrieve formatted citations for PubMed and PMC records to streamline academic writing and referencing.
- **Deep Record Inspection** — Fetch specific article metadata or full-text records using unique OAI identifiers.

### How it works

1. Subscribe to this server
2. Provide your NCBI API Key (Tool Name) and registered email
3. Start querying the world's largest repository of life sciences literature directly from your AI client

### Who is this for?

- **Researchers & Academics** — Automate literature reviews, find full-text sources, and manage citations without manual searching.
- **Data Scientists** — Harvest large-scale biomedical datasets for NLP, trend analysis, or knowledge graph construction.
- **Medical Professionals** — Quickly find peer-reviewed evidence and convert clinical identifiers into accessible research papers.


## Available Tools
- **convert_ids**: Returns JSON.

Convert between PMCIDs, PMIDs, DOIs, and Manuscript IDs
- **export_citation**: Export formatted citations for PubMed and PMC articles
- **oa_discover**: ) for PMC articles.

Discover downloadable resources from the PMC Open Access Subset
- **oai_get_record**: Get a specific OAI record from PMC
- **oai_identify**: Identify the PMC OAI-PMH repository
- **oai_list_identifiers**: Use metadataPrefix (e.g., pmc, pmc_fm, oai_dc).

List OAI identifiers for PMC articles
- **oai_list_metadata_formats**: Optionally filter by a specific identifier.

List available metadata formats in PMC OAI-PMH
- **oai_list_records**: List full OAI records for PMC articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PMC Open Access (PubMed Central)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the following PMIDs to PMCIDs: 34567890, 34567891."

**🤖 AI Agent:**
> I've converted those IDs for you. PMID 34567890 corresponds to PMCID PMC8451234 and DOI 10.1038/s41586-021-03850-x.

---

**👤 You:**
> "Find the PDF download link for PMCID PMC5334499."

**🤖 AI Agent:**
> I found the resources for PMC5334499. You can download the PDF directly from the PMC Open Access archive at the following URL: [URL].

---

**👤 You:**
> "List the metadata formats supported by the PMC OAI-PMH repository."

**🤖 AI Agent:**
> The PMC repository supports several metadata formats, including 'oai_dc' (Dublin Core), 'pmc' (Full-text XML), and 'pmc_fm' (Front matter only).


## Installation & Usage

To install and use the **PMC Open Access (PubMed Central)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pmc-open-access-pubmed-central](https://vinkius.com/mcp/pmc-open-access-pubmed-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
