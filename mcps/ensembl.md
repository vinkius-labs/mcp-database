# Ensembl MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ensembl)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ensembl-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ensembl-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access genomic data, gene trees, homologies, and cross-references from the Ensembl database directly from any AI agent.

## Description
Connect to the **Ensembl** REST API to perform advanced genomic research and biological data retrieval through natural conversation.

### What you can do

- **Comparative Genomics** — Retrieve gene trees, homologies (orthologs/paralogs), and genomic alignments across multiple species.
- **Archive & Lookup** — Fetch the latest versions of stable identifiers and look up current metadata for genes and transcripts.
- **Cross References (Xrefs)** — Link Ensembl objects to external databases using symbols (e.g., BRCA2) or specific external IDs.
- **Species Metadata** — List all available species in the Ensembl database and retrieve their specific assembly information.
- **Sequence Analysis** — Access genomic sequences by ID or region, and perform variant effect prediction (VEP) queries.

### How it works

1. Subscribe to this server
2. Enter your API configuration (use 'PUBLIC' for standard access)
3. Start querying genomic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bioinformaticians** — quickly pull gene trees and homology data without writing custom Python or R scripts
- **Genomic Researchers** — verify stable ID versions and cross-reference symbols directly from their research environment
- **Data Scientists** — automate the retrieval of genomic alignments and metadata for large-scale biological analysis


## Available Tools
- **get_alignment**: Retrieves genomic alignments for a specific region
- **get_archive_bulk**: Retrieve the latest version for a set of identifiers
- **get_archive_id**: Returns the latest version of a given identifier
- **get_ga4gh_beacon**: Beacon service for allele information
- **search_ga4gh_variants**: Search for variants using GA4GH schema
- **get_genetree**: Retrieves a gene tree for a stable identifier
- **get_homology**: Retrieves homology information by species and gene ID
- **get_info_assembly**: List available assemblies and chromosomes for a species
- **get_info_rest**: Current version of the Ensembl REST API
- **get_info_species**: Lists all available species and their metadata
- **get_ld**: Compute Linkage Disequilibrium (LD) values
- **get_lookup_bulk**: Bulk lookup for multiple identifiers
- **get_lookup_id**: Find the species and database for a single identifier
- **get_map_cdna**: Convert cDNA coordinates to genomic coordinates
- **get_map**: Convert coordinates from one assembly version to another
- **get_ontology_id**: Search for an ontological term by its identifier
- **get_overlap_region**: ) overlapping a region.

Retrieve features overlapping a specific region
- **ping**: Check if the service is alive
- **get_sequence_id**: Request sequence by stable identifier
- **get_sequence_region**: Request genomic sequence by region
- **get_taxonomy_id**: Search for a taxonomic term by ID or name
- **get_variation**: Retrieve variant features, genotypes, and population data
- **get_vep_bulk**: Bulk consequence prediction for multiple regions
- **get_vep_hgvs**: Fetch consequences for a variant in HGVS notation
- **get_vep_id**: Fetch consequences for a variant identifier (e.g., rsID)
- **get_xrefs_id**: Retrieve external references for an Ensembl identifier
- **get_xrefs_symbol**: Look up an external symbol and return linked Ensembl objects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ensembl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest version of the Ensembl identifier ENSG00000139618?"

**🤖 AI Agent:**
> I've checked the archive for ENSG00000139618. The latest version is version 11, which is currently active in the latest assembly.

---

**👤 You:**
> "Find all orthologues for the human gene ENSG00000139618 in mouse."

**🤖 AI Agent:**
> Searching homologies... I found 1 high-confidence orthologue in Mus musculus: ENSMUSG00000041147 (Brca2). Would you like the alignment details?

---

**👤 You:**
> "List all species currently available in the Ensembl database."

**🤖 AI Agent:**
> I've retrieved the species list. There are over 300 species available, including Homo sapiens, Mus musculus, Danio rerio, and many others. Do you want to filter by a specific taxon?


## Installation & Usage

To install and use the **Ensembl** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ensembl](https://vinkius.com/mcp/ensembl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
