# PubChem MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubchem)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pubchem-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pubchem-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 116M+ chemical compounds with molecular properties, SMILES notation, formulas, and drug-like properties from the world's largest free chemistry database.

## Description
Connect your AI agent to **PubChem** — the world's largest open chemistry database, maintained by the National Center for Biotechnology Information (NCBI/NIH).

### What you can do

- **Compound Search** — Find chemical compounds by common name (aspirin, caffeine, glucose), IUPAC name, or CAS number across 116M+ indexed compounds
- **CID Lookup** — Get comprehensive molecular data for any compound by its PubChem Compound ID including formula, weight, SMILES, InChI, and physicochemical properties
- **Formula Search** — Find all compounds matching a specific molecular formula (e.g., C9H8O4 for aspirin)

### How it works

1. Subscribe to this server
2. Start searching compounds immediately — no API key required

### Who is this for?

- **Medicinal Chemists** — quickly retrieve molecular properties and drug-like characteristics for lead compounds
- **Pharmacy Students** — look up drug structures, formulas, and physicochemical data during coursework
- **Biochemistry Researchers** — identify compounds by formula and explore metabolite databases


## Available Tools
- **get_pubchem_compound**: Get full chemical data for a PubChem compound by CID
- **search_pubchem_formula**: g. C9H8O4, C8H10N4O2, H2O) and find matching compounds.

Find compounds by molecular formula
- **search_pubchem**: Returns molecular formula, weight, SMILES, InChI, XLogP, hydrogen bond donors/acceptors, and complexity. Try: aspirin, caffeine, glucose, penicillin, dopamine.

Search PubChem for chemical compounds by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubChem** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the molecular properties of aspirin?"

**🤖 AI Agent:**
> Aspirin (CID 2244): Formula C9H8O4, MW 180.16, SMILES CC(=O)OC1=CC=CC=C1C(O)=O, XLogP 1.2, H-bond donors: 1, H-bond acceptors: 4. Passes Lipinski's Rule of Five — classified as drug-like.

---

**👤 You:**
> "Search for compounds with the molecular formula C8H10N4O2."

**🤖 AI Agent:**
> Found compounds matching C8H10N4O2: Primary result is Caffeine (CID 2519) — the alkaloid found in coffee, tea, and chocolate. MW: 194.19, SMILES: CN1C=NC2=C1C(=O)N(C(=O)N2C)C. Also found: Theophylline (CID 2153) — used as bronchodilator for asthma treatment.

---

**👤 You:**
> "Get the full chemical details for PubChem compound CID 5090."

**🤖 AI Agent:**
> CID 5090: Metformin — Formula C4H11N5, MW 129.16, SMILES CN(C)C(=N)NC(=N)N. XLogP: -1.4 (highly water-soluble). H-bond donors: 3, acceptors: 3. Widely used as first-line treatment for type 2 diabetes. Molecular complexity: 95.


## Installation & Usage

To install and use the **PubChem** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubchem](https://vinkius.com/mcp/pubchem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
