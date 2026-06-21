# EBI PDBe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebi-pdbe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ebi-pdbe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ebi-pdbe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore 3D protein structures, ligand interactions, and molecular assemblies from the Protein Data Bank in Europe.

## Description
Connect to the **PDBe (Protein Data Bank in Europe) API** and access the world's most comprehensive repository of experimentally determined 3D macromolecular structures.

### What you can do

- **Structure Summaries** — Get titles, authors, deposition dates, resolution, and experimental methods for any PDB entry
- **Molecular Entities** — Retrieve protein chains, nucleic acids, ligands, their sequences, source organisms, and gene names
- **Binding Sites & Ligands** — Access ligand binding pocket residues, small molecule ligands with formulas and weights
- **Quality Assessment** — Check resolution, R-factors, and overall quality scores for structure reliability
- **UniProt Mappings** — Map between UniProt sequence positions and PDB residue numbers
- **Biological Assemblies** — Understand quaternary structure — monomer, dimer, tetramer, or higher-order complexes
- **Structure Search** — Full-text Solr search across 200+ PDB metadata fields
- **Publications** — Find primary citations, PubMed IDs, and related structural studies

### How it works

1. Subscribe to this server
2. No API key required — the PDBe API is fully public
3. Start querying 3D structures from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a structural biology research assistant with direct access to every experimentally determined protein structure. All data is sourced from the official PDBe REST API maintained by EMBL-EBI.

### Who is this for?

- **Structural Biologists** — retrieve structure metadata, quality assessments, and experimental parameters without downloading coordinate files
- **Drug Discovery Scientists** — identify binding sites, ligand interactions, and cofactors for rational drug design
- **Bioinformaticians** — cross-reference sequence data with 3D structural annotations via UniProt mappings
- **Educators & Students** — explore real macromolecular structures for teaching protein chemistry and structural biology


## Available Tools
- **get_assemblies**: Returns assembly IDs, composition (which entities and how many copies), preferred assembly flag, and form description. Critical for understanding whether a protein functions as a monomer, dimer, tetramer, or higher-order complex.

Get biological assembly information (quaternary structure)
- **get_binding_sites**: Critical for drug discovery, molecular docking, and understanding protein-ligand interactions.

Get ligand binding site residues and interactions
- **get_cofactors**: Cofactors like heme, NAD+, FAD, and metal ions are essential for enzyme catalysis and protein function.

Get cofactor and prosthetic group annotations
- **get_experiment**: Get experimental method details for a structure
- **get_ligand_monomers**: Returns chemical component IDs, names, molecular formulas, molecular weights, and their chain/residue positions. Essential for drug discovery and understanding protein-small molecule interactions.

Get small molecule ligands bound in the structure
- **get_modified_residues**: Shows the parent compound ID and modification name.

Get non-standard amino acids and nucleotides
- **get_molecules**: Returns entity IDs, molecule types, names, chain assignments, sequence lengths, molecular weights, source organisms, and gene names.

Get molecular entities (chains, polymers) in a structure
- **get_mutated_residues**: Shows the original residue, mutated residue, chain, and position. Essential for understanding how the crystallized construct differs from the native protein.

Get engineered mutations vs. wild-type sequence
- **get_publications**: Useful for finding the primary citation and methodology papers for a structure.

Get associated journal publications and PubMed IDs
- **get_quality_scores**: The first thing a structural biologist checks when evaluating a structure for reliability.

Get global quality metrics for a structure
- **get_related_entries**: Useful for discovering alternative conformations, mutants, or complexes of the same protein that have been structurally characterized.

Get related PDB entries citing the same publications
- **get_residue_listing**: Shows residue names, numbers (both PDB and author numbering), organized by entity and chain. Returns a sample of the first 20 residues per chain for efficiency.

Get full residue-level inventory per chain
- **get_secondary_structure**: Shows the count of helices and strands per chain, organized by molecular entity. Essential for understanding protein fold topology.

Get helix, sheet, and coil assignments per residue
- **get_summary**: Use a 4-character PDB ID such as 1cbs, 4hhb, 6lu7.

Get PDB entry summary with title, authors, and resolution
- **get_uniprot_mapping**: Returns UniProt accessions, chain assignments, and start/end position mappings. Essential for cross-referencing between protein sequence databases and 3D structural data.

Get UniProt to PDB residue mappings
- **search_structures**: Use natural language queries like "insulin receptor kinase", "SARS-CoV-2 spike protein", "cryo-EM resolution<3", or specific organism names. Returns PDB IDs, titles, methods, resolutions, and organisms.

Search PDB structures with full-text queries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EBI PDBe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the structure summary and quality of the SARS-CoV-2 main protease (6lu7)."

**🤖 AI Agent:**
> I've retrieved the structure summary for 6LU7, the SARS-CoV-2 main protease. It was determined by X-ray crystallography at 2.16 Å resolution. The structure contains the protease in complex with an inhibitor, providing key insights for antiviral drug design. The quality metrics show good geometry and reliable electron density.

---

**👤 You:**
> "What ligands are bound in the hemoglobin structure 4hhb?"

**🤖 AI Agent:**
> I've retrieved the ligand data for hemoglobin (4HHB). The structure contains heme (protoporphyrin IX) groups as cofactors bound to each of the four globin chains. The heme groups contain iron atoms essential for oxygen binding. I also found the binding site residues that coordinate the heme cofactors.

---

**👤 You:**
> "Search for cryo-EM structures of ribosome complexes."

**🤖 AI Agent:**
> I've found multiple ribosome structures determined by cryo-electron microscopy. The search returned entries from various organisms including E. coli, human, and yeast ribosomes at resolutions ranging from 2.0 to 4.0 Å. These include 70S and 80S ribosomes in complex with mRNA, tRNA, and various translation factors.


## Installation & Usage

To install and use the **EBI PDBe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebi-pdbe](https://vinkius.com/mcp/ebi-pdbe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
