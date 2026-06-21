# GenBank/NCBI API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genbankncbi-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/genbankncbi-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/genbankncbi-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Access genomic data — audit sequences, proteins, and UIDs via IA.

## Description
Empower your AI agent to orchestrate your entire biological research and genomic auditing workflow with the **GenBank/NCBI API**, the authoritative source for molecular biology data from the National Center for Biotechnology Information. By connecting NCBI's E-utilities to your agent, you transform complex sequence searches into a natural conversation. Your agent can instantly retrieve sequence UIDs, audit bibliographic summaries, and query protein metadata without you ever touching a bioinformatics portal. Whether you are conducting evolutionary research or managing laboratory constraints, your agent acts as a real-time genomic consultant, ensuring your data is always verified and precise.

### What you can do

- **Sequence Auditing** — Search for thousands of genetic sequences by keyword and retrieve high-resolution metadata, including UIDs and titles.
- **Database Oversight** — Audit multiple NCBI databases like 'nuccore' or 'protein' to understand the thematic distribution of biological data instantly.
- **Summary Discovery** — Query technical and bibliographic summaries for specific sequence IDs to assist in deep-dive archival classification.
- **Metadata Intelligence** — Retrieve unique identifiers and caption details for any biological record to assist in scientific auditing.
- **Operational Monitoring** — Check API status to ensure your bioinformatics research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (NCBI E-utilities is a free and open service)
3. Start managing your genomic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Biologists & Geneticists** — monitor sequence data and retrieve official metadata straight from your workflow.
- **Bioinformaticians** — verify UIDs and audit molecular patterns without manual searching.
- **Students & Researchers** — perform rapid audits of protein properties and identify relevant biological markers through natural language.
- **Operations Leads** — automate scientific data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_api_status**: Check if the NCBI E-utilities service is operational
- **get_ncbi_summary**: Get a summary for a specific NCBI sequence ID
- **list_ncbi_databases**: List all available NCBI databases
- **search_ncbi_sequences**: g., nuccore, protein) based on a query term.

Search for biological sequences in an NCBI database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GenBank/NCBI API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'human insulin' in the 'protein' database using NCBI."

**🤖 AI Agent:**
> I've retrieved several matching records for human insulin! Notable UIDs include [UID 1] and [UID 2]. Would you like the full technical summary or the bibliographic metadata for any of these identifiers?

---

**👤 You:**
> "Get the summary for NCBI UID '123456' in 'nuccore'."

**🤖 AI Agent:**
> I've retrieved the summary for UID 123456! It is a nucleotide sequence titled [Title]. I can provide the publication date and caption metadata to help you identify it in your workflow.

---

**👤 You:**
> "List all available NCBI databases."

**🤖 AI Agent:**
> I've scanned the database catalog from NCBI! There are over 30 biological databases available, including PubMed, Protein, and Nucleotide. I can help you search for specific records in any of these thematic clusters.


## Installation & Usage

To install and use the **GenBank/NCBI API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genbankncbi-api](https://vinkius.com/mcp/genbankncbi-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
