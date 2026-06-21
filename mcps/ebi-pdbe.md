# EBI PDBe MCP Server

Explore 3D protein structures, ligand interactions, and molecular assemblies from the Protein Data Bank in Europe.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ebi-pdbe)

## Overview
**Category:** the-unthinkable
**Tools Count:** 16

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


## Installation & Usage

To install and use the **EBI PDBe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebi-pdbe](https://vinkius.com/mcp/ebi-pdbe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
