# EPA Computational Toxicology MCP Server

Access the US EPA's CompTox Chemicals Dashboard data — search for chemicals, properties, hazard summaries, and exposure data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-computational-toxicology)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect to the US Environmental Protection Agency's (EPA) Center for Computational Toxicology and Exposure (CCTE) and explore a massive repository of chemical data through natural conversation.

### What you can do

- **Chemical Search** — Find substances by name, CAS Registry Number (CASRN), or DTXSID
- **Physicochemical Properties** — Retrieve melting points, boiling points, logP, and water solubility
- **Hazard Assessments** — Access toxicity values, NOAELs, and points-of-departure from ToxValDB
- **Exposure Predictions** — Explore predicted exposure levels and product use categories via ExpoCast and CPDat
- **Bioactivity Screening** — Analyze ToxCast/Tox21 high-throughput screening results for thousands of assays
- **Environmental Fate** — Check persistence, transport, and biodegradation metrics

### How it works

1. Subscribe to this server
2. Enter your free EPA API Key (request it by emailing `ccte_api@epa.gov`)
3. Start investigating chemical safety and properties directly from your agent

This tool is essential for toxicologists, environmental scientists, and regulatory professionals who need instant access to high-quality chemical data.

### Who is this for?

- **Toxicologists** — quickly gather hazard and bioactivity data for risk assessments
- **Environmental Scientists** — analyze fate and transport properties of contaminants
- **Product Safety Teams** — check chemical exposure and product use profiles
- **Researchers** — retrieve identifiers and synonyms for chemical lists


## Available Tools
- **get_bioactivity_summary**: Retrieve a summary of high-throughput screening results from ToxCast/Tox21 assays
- **get_chemical_details**: Get comprehensive metadata and identification details for a specific chemical using its DTXSID
- **get_chemical_lists**: Identify which chemical lists (regulatory, research, or commercial) this chemical belongs to
- **get_chemical_synonyms**: Retrieve all known synonyms and alternative names for a specific chemical
- **get_exposure_summary**: Retrieve predicted exposure levels and product use data (ExpoCast/CPDat)
- **get_fate_and_transport**: Retrieve environmental fate and transport data (e.g., half-life, bioconcentration)
- **get_hazard_summary**: Retrieve a summary of toxicity values and hazard assessment data from ToxValDB
- **get_physicochemical_properties**: Retrieve predicted and experimental physicochemical properties (e.g., melting point, logP, solubility) for a chemical
- **search_chemical_by_casrn**: Search for chemicals by their CAS Registry Number (CASRN)
- **search_chemical_by_name**: Search for chemicals by common, IUPAC, or synonym names in the EPA CompTox database


## Installation & Usage

To install and use the **EPA Computational Toxicology** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-computational-toxicology](https://vinkius.com/mcp/epa-computational-toxicology)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
