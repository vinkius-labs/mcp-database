# EPA Computational Toxicology MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-computational-toxicology)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epa-computational-toxicology-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epa-computational-toxicology-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access the US EPA's CompTox Chemicals Dashboard data — search for chemicals, properties, hazard summaries, and exposure data.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPA Computational Toxicology** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the chemical properties of Bisphenol A."

**🤖 AI Agent:**
> I've found Bisphenol A (DTXSID7020182). Its properties include a melting point of 158°C, water solubility of 120 mg/L, and a logP of 3.32.

---

**👤 You:**
> "What is the hazard summary for CAS 80-05-7?"

**🤖 AI Agent:**
> For CAS 80-05-7, the hazard summary indicates concerns for endocrine disruption and reproductive toxicity, with ToxValDB listing several points-of-departure for developmental endpoints.

---

**👤 You:**
> "Find predicted exposure data for DTXSID7020182."

**🤖 AI Agent:**
> Retrieving exposure data... Predicted geometric mean intake for this substance is 1.2e-4 mg/kg-bw/day. Common product categories include 'Food Packaging' and 'Polymer production'.


## Installation & Usage

To install and use the **EPA Computational Toxicology** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-computational-toxicology](https://vinkius.com/mcp/epa-computational-toxicology)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
