# RCSB PDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rcsb-pdb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rcsb-pdb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rcsb-pdb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore 220K+ 3D molecular structures — search proteins, DNA, and RNA by name, experimental method, resolution, and bound ligands from the Protein Data Bank.

## Description
Connect your AI agent to the **RCSB Protein Data Bank** — the world's repository of experimentally determined 3D structural data for biological macromolecules.

### What you can do

- **Structure Search** — Find protein, DNA, and RNA structures by name, function, disease association, or organism across 220K+ experimentally determined entries
- **PDB Entry Lookup** — Get complete structural details by 4-character PDB ID (e.g., 1HHO for hemoglobin, 6LU7 for SARS-CoV-2 main protease) including experimental method, resolution, and bound molecules

### How it works

1. Subscribe to this server
2. Start searching molecular structures immediately — no API key required

### Who is this for?

- **Structural Biologists** — quickly access experimental metadata, resolution, and method details for molecular structures
- **Drug Discovery Teams** — find protein-ligand co-crystal structures for structure-based drug design and virtual screening
- **Biochemistry Students** — understand protein architecture by exploring real experimental structures with annotations


## Available Tools
- **get_pdb_structure**: PDB IDs are 4-character codes like 1HHO, 6LU7, 7BNN.

Get full structural details by PDB ID
- **search_pdb**: Returns PDB ID, title, experimental method (X-ray, Cryo-EM, NMR), resolution, authors, and bound ligands. Essential for drug discovery and structural biology.

Search 220K+ 3D molecular structures in the Protein Data Bank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RCSB PDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the structure of the SARS-CoV-2 main protease."

**🤖 AI Agent:**
> Found PDB 6LU7: Crystal structure of SARS-CoV-2 main protease (Mpro) in complex with inhibitor N3. Method: X-ray Diffraction, Resolution: 2.16 Å. Authors: Jin et al. Released: 2020-02-05. Ligands: N3 (peptide-like inhibitor). This was one of the first high-resolution structures of the COVID-19 drug target. View: rcsb.org/structure/6LU7

---

**👤 You:**
> "Get full structural details for PDB entry 1HHO — what protein is it?"

**🤖 AI Agent:**
> PDB 1HHO: Deoxy Human Hemoglobin — the oxygen-carrying protein in red blood cells. Method: X-ray Diffraction, Resolution: 2.10 Å. Authors: Fermi et al. Released: 1984-07-20. Contains 4 polymer chains (2 alpha, 2 beta subunits) with heme (protoporphyrin IX containing iron) bound as cofactor.

---

**👤 You:**
> "Find all cryo-EM structures of ribosome complexes."

**🤖 AI Agent:**
> Found 10 ribosome structures determined by Cryo-EM. Highlights: Human 80S ribosome (PDB 4UG0) at 3.6 Å resolution — the molecular machine that translates mRNA into proteins. Also found: E. coli 70S ribosome with antibiotics bound (critical for understanding antibiotic mechanisms), and mitochondrial ribosome structures.


## Installation & Usage

To install and use the **RCSB PDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rcsb-pdb](https://vinkius.com/mcp/rcsb-pdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
