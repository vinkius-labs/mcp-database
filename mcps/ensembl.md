# Ensembl MCP Server

Access genomic data, gene trees, homologies, and cross-references from the Ensembl database directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ensembl)

## Overview
**Category:** databases
**Tools Count:** 27

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


## Installation & Usage

To install and use the **Ensembl** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ensembl](https://vinkius.com/mcp/ensembl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
