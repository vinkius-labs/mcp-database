# EBI Proteins API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebi-proteins-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Query the UniProt knowledge base for protein sequences, annotations, and functional data across millions of characterized entries.

## Description
Connect to the **EMBL-EBI Proteins API** and access comprehensive protein biology data from one of the world's leading bioinformatics institutes.

### What you can do

- **Protein Retrieval** — Fetch complete protein entries by UniProt accession with names, organisms, gene information, sequences, and cross-references
- **Sequence Features** — Retrieve annotated domains, binding sites, active sites, signal peptides, transmembrane regions, and disulfide bonds for any protein
- **Genetic Variants** — Access curated variants from UniProtKB aggregated with large-scale studies including ClinVar, gnomAD, 1000 Genomes, COSMIC, and TOPMed
- **Proteomics & PTMs** — Query mass-spectrometry peptide evidence and post-translational modifications from PeptideAtlas, MaxQB, EPD, and ProteomicsDB
- **Mutagenesis** — Explore curated mutagenesis experiments with detailed phenotypic effect descriptions
- **Proteomes & Taxonomy** — Search reference proteomes and navigate the taxonomy tree by ID or organism name
- **Genome Coordinates** — Map proteins to genome positions on GRCh38/GRCh37 with Ensembl gene, transcript, and translation IDs

### How it works

1. Subscribe to this server
2. No API key required — the EBI Proteins API is fully public
3. Start querying protein data from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a molecular biology research assistant with direct access to the entire UniProt protein knowledge base. All data is sourced from the official EMBL-EBI Proteins REST API.

### Who is this for?

- **Molecular Biologists** — retrieve protein sequences, domain architectures, and functional annotations without navigating complex web databases
- **Clinical Geneticists** — access aggregated variant data from ClinVar, gnomAD, and COSMIC for variant interpretation and pathogenicity assessment
- **Structural Biologists** — query sequence features, binding sites, and mutagenesis data to guide experimental design
- **Bioinformaticians** — programmatically access proteomes, taxonomy, and genome coordinate mappings for pipeline integration


## Available Tools (16)
- **get_antigen**: These are peptide regions used for antibody generation, indicating experimentally validated protein expression targets. Useful for immunology and antibody-based research.

Get antigen sequences from Human Protein Atlas
- **get_coordinates**: Returns Ensembl gene, transcript, and translation IDs along with chromosome, start/end positions, and strand information. Essential for bridging protein annotations with genomic data.

Get genome coordinate mappings for a protein
- **get_protein_features**: Features include domains, binding sites, active sites, signal peptides, transmembrane regions, disulfide bonds, glycosylation sites, and more. Each feature has start/end positions and evidence counts.

Get sequence feature annotations for a protein
- **get_genecentric**: Shows canonical protein and related protein count for each gene. Use with a UniProt Proteome ID (e.g. UP000005640).

Get the gene-centric view of a proteome
- **get_mutagenesis**: Each entry includes the wild-type and mutant residues, position, and a description of the functional impact. Critical for understanding structure-function relationships.

Get mutagenesis experiments and phenotypic effects
- **get_protein**: Use a UniProt accession such as P12345, Q9Y6K9, or P53_HUMAN.

Retrieve a full protein entry by UniProt accession
- **get_proteome**: Returns taxonomy, protein count, gene count, reference status, and component information. Use IDs like UP000005640 for human proteome or UP000000589 for mouse.

Get a specific proteome by UniProt Proteome ID
- **get_proteomics**: Shows which peptides have been experimentally detected and whether they are unique to this protein. Essential for validating protein expression.

Get mass-spectrometry proteomics data for a protein
- **get_proteomics_ptm**: Provides residue-level PTM positions with evidence counts.

Get post-translational modifications from mass-spec data
- **get_taxonomy**: Returns scientific name, common name, rank, lineage, parent, and children nodes. Use IDs like 9606 for human, 10090 for mouse, 562 for E. coli.

Get taxonomy node details by NCBI taxon ID
- **get_variation**: Each variant includes wild-type and mutant residues, clinical significance, consequence type (e.g. missense, nonsense), and cross-references. Critical for clinical genomics and variant interpretation.

Get genetic variants for a protein from multiple sources
- **search_features_by_type**: Valid types include: DOMAIN, BINDING, ACTIVE_SITE, SIGNAL, TRANSMEM, DISULFID, CARBOHYD, MOD_RES, VARIANT, MUTAGEN, REGION, MOTIF, SITE, REPEAT, COILED, COMPBIAS, HELIX, STRAND, TURN.

Search features by type across proteins
- **search_proteins**: You can combine gene name (e.g. TP53), organism (e.g. human, 9606), keyword (e.g. kinase), or accession. Returns a summarized list of matching proteins with names, organisms, and sequence lengths.

Search proteins by gene name, organism, or keyword
- **search_proteomes**: Returns proteome IDs, taxonomy, protein counts, gene counts, and reference proteome status. Use queries like "homo sapiens", "escherichia coli", "arabidopsis".

Search proteomes by organism name
- **search_taxonomy**: Returns matching taxonomy entries with scientific names, common names, taxon IDs, and ranks. Useful for finding the correct taxon ID before querying proteins or proteomes for a specific organism.

Search taxonomy by organism name
- **search_variation**: g. large_scale_study, uniprot, mixed), consequence type (e.g. missense, stop gained), and wild-type residue. Use this to find clinically relevant variants across the proteome.

Search variants by consequence type, source, or residue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EBI Proteins API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get all known genetic variants for the TP53 tumor suppressor protein."

**🤖 AI Agent:**
> I've retrieved the variant data for TP53 (P04637) from the EBI Proteins API. The protein has hundreds of documented variants aggregated from UniProtKB, ClinVar, gnomAD, COSMIC, and other sources. These include missense mutations in the DNA-binding domain (residues 100-290) which are the most clinically significant, along with their pathogenicity classifications and population frequencies.

---

**👤 You:**
> "Show me the domain architecture and binding sites of the EGFR protein."

**🤖 AI Agent:**
> I've retrieved the sequence features for EGFR (P00533). The protein contains multiple annotated domains including the extracellular ligand-binding domain, furin-like cysteine-rich domains, a transmembrane region, and the intracellular tyrosine kinase domain. Key binding sites include the ATP-binding site in the kinase domain and EGF receptor-binding regions. I also found signal peptides, glycosylation sites, and disulfide bonds.

---

**👤 You:**
> "Map the BRCA1 protein to its genome coordinates on GRCh38."

**🤖 AI Agent:**
> I've mapped BRCA1 (P38398) to genome coordinates. The protein maps to chromosome 17 on the GRCh38 assembly, with Ensembl gene ID ENSG00000012048 and transcript ID ENST00000357654. The coding region spans a large genomic interval on the reverse strand, reflecting BRCA1's complex exon structure. This mapping allows you to cross-reference protein-level variant annotations with genomic positions.


## ❓ FAQ

**Q: Do I need an API key to use this server?**
No. The EMBL-EBI Proteins API is completely public and requires no authentication. Simply subscribe to this server and enter any placeholder value in the API key field to start querying protein data immediately.

**Q: What kind of variant data is available?**
The server aggregates genetic variants from multiple authoritative sources: UniProtKB curated variants, ClinVar clinical significance data, gnomAD population frequencies, 1000 Genomes Project, COSMIC somatic mutations, TOPMed whole-genome sequencing, ExAC exome data, and TCGA cancer variants. Each variant includes consequence type, clinical significance, and source cross-references.

**Q: Can I map protein positions to genome coordinates?**
Yes. The get_coordinates tool maps any UniProt protein to reference genome coordinates on GRCh38 and GRCh37 assemblies. It returns Ensembl gene, transcript, and translation identifiers along with chromosome, start/end positions, and strand orientation. This bridges the gap between protein-level annotations and genomic-level analyses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebi-proteins-api](https://vinkius.com/mcp/ebi-proteins-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EBI Proteins API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ebi-proteins-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EBI Proteins API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebi-proteins-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
