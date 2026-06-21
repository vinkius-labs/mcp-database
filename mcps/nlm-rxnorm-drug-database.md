# NLM RxNorm (Drug Database) MCP Server

Access the NLM RxNorm database to search for drugs, retrieve RxCUIs, and inspect standardized drug properties and identifiers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nlm-rxnorm-drug-database)

## Overview
**Category:** databases
**Tools Count:** 21

## Description
Connect your AI agent to the **National Library of Medicine (NLM) RxNorm** database. This server provides comprehensive access to standardized drug nomenclature and relationships, allowing for precise identification and analysis of pharmaceutical products.

### What you can do

- **Drug Search** — Find RxNorm Concept Unique Identifiers (RxCUIs) by name, identifier (NDC, ATC, SNOMEDCT), or approximate matching using `find_rxcui_by_string` and `find_rxcui_by_id`.
- **Property Inspection** — Retrieve detailed drug properties, including names, synonyms, and attributes categorized by source via `get_all_properties`.
- **Relationship Mapping** — Explore related concepts and term types (TTY) to understand drug hierarchies and ingredients using `get_all_related_info`.
- **Spelling Correction** — Get suggestions for misspelled drug names to ensure accurate queries with `get_spelling_suggestions`.
- **NDC & Identifier Lookup** — Map external codes to RxNorm standards for interoperability.

### How it works

1. Subscribe to this server
2. Enter your NLM UTS API Key
3. Start querying drug data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Developers** — Integrate standardized drug data into clinical decision support tools.
- **Medical Researchers** — Analyze drug relationships and properties using a trusted, standardized vocabulary.
- **Data Scientists** — Map disparate drug datasets to a common RxNorm standard for analysis.


## Available Tools
- **find_related_ndcs**: Find NDCs related by concept, drug, or NDC product
- **find_rxcui_by_id**: Search for an identifier and return associated RxCUIs
- **find_rxcui_by_string**: Search for a drug by name from any vocabulary in RxNorm
- **find_similar_classes_by_drug_list**: Identify classes with drug members similar to a provided list of RxCUIs
- **get_all_properties**: Return detailed properties for an RxNorm concept
- **get_all_related_info**: Retrieve all concepts related to a specified RxCUI
- **get_all_rxterm_info**: Return display names, synonyms, strengths, and routes for an RxCUI
- **get_approximate_match**: Find concepts and atom IDs that approximately match a query string
- **get_class_by_rxnorm_drug_id**: Return the classes containing a specific drug
- **get_class_members**: g., ATC, MeSH, VA Class).

Return all drug members of a specified class
- **get_drugs**: ) related to an ingredient or brand name.

Return drug products related to a specified name
- **get_ndc_properties**: Return detailed metadata for an NDC
- **get_ndc_status**: Return the status and history of an NDC
- **get_ndcs**: Return active NDCs associated with an RxNorm concept
- **get_related_by_relationship**: g., tradename_of).

Retrieve concepts directly related by a specific relationship type
- **get_related_by_type**: g., IN, SBD, SCD).

Retrieve related concepts of specific term types
- **get_rx_concept_properties**: Return basic properties for an RxNorm concept
- **get_rx_property**: Retrieve a specific property value for a concept
- **get_rxterm_display_name**: Return the RxTerms display name for a concept
- **get_rxcui_history_status**: Return the status, attributes, and history of a concept
- **get_spelling_suggestions**: Return strings similar to a specified string for auto-correction


## Installation & Usage

To install and use the **NLM RxNorm (Drug Database)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nlm-rxnorm-drug-database](https://vinkius.com/mcp/nlm-rxnorm-drug-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
