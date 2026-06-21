# EBI InterPro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebi-interpro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Classify protein sequences into families, predict functional domains, and explore evolutionary relationships across species.

## Description
Connect to the **InterPro API** and access the world's most comprehensive resource for protein family, domain, and functional site classification.

### What you can do

- **Domain Classification** — Retrieve detailed InterPro entry information including family/domain descriptions, GO terms, and member database cross-references
- **Multi-Database Access** — Query entries from Pfam, CDD, SMART, Prosite, PANTHER, Gene3D, HAMAP, and more through a unified interface
- **Protein Annotation** — Find all InterPro domains, families, and sites annotated on any UniProt protein
- **Structure Mapping** — Discover PDB structures containing proteins that match specific InterPro entries
- **Taxonomic Distribution** — Explore which organisms contain proteins matching a domain or family — essential for evolutionary biology
- **Proteome Coverage** — Assess domain annotation coverage for complete proteomes
- **Clan Analysis** — Navigate Pfam clan hierarchies to understand super-family relationships

### How it works

1. Subscribe to this server
2. No API key required — the InterPro API is fully public
3. Start classifying proteins from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a protein domain expert with access to InterPro's unified classification of protein families from 13+ member databases. All data is sourced from the official InterPro REST API maintained by EMBL-EBI.

### Who is this for?

- **Molecular Biologists** — classify unknown proteins into families and predict their functional domains
- **Evolutionary Biologists** — explore taxonomic distributions of protein domains across the tree of life
- **Structural Biologists** — find 3D structures containing specific protein domains for comparative analysis
- **Bioinformaticians** — integrate protein family classifications into automated annotation pipelines


## Available Tools (16)
- **get_cdd_entry**: CDD provides curated models for protein domain families and includes additional alignment and structure data. Use accessions like cd00001.

Get CDD (Conserved Domain Database) entry details
- **get_clan**: Returns clan accession, name, description, and member counts. Use Pfam clan accessions like CL0001.

Get Pfam clan (super-family grouping) details
- **get_entry**: Returns name, type (family, domain, homologous superfamily, repeat, site), description, Gene Ontology terms, member database cross-references, and literature count. Use accessions like IPR000001, IPR036291.

Get InterPro entry metadata for a family or domain
- **get_entry_proteins**: Returns protein accessions, names, lengths, and source organisms. Useful for finding all members of a protein family across the UniProt database.

Get all proteins matching an InterPro entry
- **get_entry_structures**: Returns PDB IDs, names, experiment types, and resolutions. Useful for finding structural representatives of a protein family or domain.

Get all PDB structures matching an InterPro entry
- **get_entry_taxonomy**: Returns taxonomy nodes with names, ranks, and protein counts. This answers the evolutionary biology question "which organisms have this domain/family?" and is essential for understanding protein evolution and conservation.

Get taxonomic distribution of an InterPro entry
- **get_pfam_entry**: Pfam is the most widely used protein domain database. Use accessions like PF00069 (kinase domain), PF00076 (RRM domain).

Get Pfam domain or family details
- **get_protein**: Returns the protein name, length, source organism, evidence level, fragment status, and counters for how many InterPro entries, Pfam domains, structures, and taxa are associated with it.

Get protein details with all domain and family assignments
- **get_protein_entries**: This is the key tool for understanding "what domains does my protein have?" — the fundamental question in protein characterization.

Get all InterPro entries matching a specific protein
- **get_proteome**: Returns proteome ID, organism name, strain, reference status, and counters for associated entries and proteins. Use UniProt proteome IDs like UP000005640 (human).

Get proteome details with domain coverage statistics
- **get_structure**: Use a 4-character PDB ID like 1cbs or 4hhb.

Get a PDB structure with mapped InterPro annotations
- **get_taxonomy**: Returns the organism name, rank, lineage, number of children taxa, and counters for associated InterPro entries and proteins. Use IDs like 9606 (human), 10090 (mouse), 562 (E. coli).

Get taxonomic node with entry and protein counts
- **list_entry_databases**: Shows the number of entries in each database. Useful for understanding the scope of available domain and family annotations.

List all InterPro member databases and entry counts
- **search_entries**: Optionally filter by entry type: family, domain, homologous_superfamily, repeat, or site. Returns accessions, names, types, and protein/structure counts. Use queries like "kinase", "zinc finger", "immunoglobulin".

Search InterPro entries by keyword and type
- **search_proteins**: Returns UniProt accessions, names, lengths, organisms, and annotation counts. Use queries like "insulin", "hemoglobin", "BRCA1".

Search proteins in InterPro by name or keyword
- **search_taxonomy**: Returns taxon IDs, names, ranks, and annotation counts. Use queries like "human", "drosophila", "arabidopsis", "saccharomyces".

Search taxonomy by organism name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EBI InterPro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What domains and families does the human TP53 protein belong to?"

**🤖 AI Agent:**
> I've retrieved all InterPro annotations for TP53 (P04637). The protein is classified into the p53 tumor suppressor family (IPR002117), contains a p53 DNA-binding domain (IPR011615), a p53 tetramerization domain (IPR010991), and a transactivation domain. These domains are conserved across vertebrates and define the functional architecture of p53 as a transcription factor and tumor suppressor.

---

**👤 You:**
> "Show me all member databases in InterPro and how many entries each has."

**🤖 AI Agent:**
> I've retrieved the InterPro database overview. The platform integrates 13+ member databases: Pfam leads with over 20,000 families and domains, followed by PANTHER, Gene3D, and CDD with thousands of entries each. SMART, Prosite, HAMAP, PRINTS, PIRSF, SFLD, NCBIfam, and AntiFam complete the collection. InterPro itself has over 46,000 integrated entries that unify signatures across these databases.

---

**👤 You:**
> "Which organisms have the kinase domain PF00069?"

**🤖 AI Agent:**
> I found the Pfam entry PF00069 (protein kinase domain) and retrieved its InterPro integration (IPR000719). The taxonomic distribution shows this domain is universally conserved across all kingdoms of life — from bacteria and archaea to plants, fungi, and animals. The human genome alone contains hundreds of kinase domain-containing proteins, making this one of the most expanded protein families in eukaryotic evolution.


## ❓ FAQ

**Q: Do I need an API key?**
No. The InterPro API is completely public and requires no authentication. Enter any placeholder value in the API key field to activate the server immediately.

**Q: What databases does InterPro integrate?**
InterPro integrates 13+ member databases including Pfam (protein families), CDD (conserved domains from NCBI), SMART (signalling domains), Prosite (patterns and profiles), PANTHER (evolutionary classification), Gene3D (structural domains from CATH), HAMAP (microbial families), PRINTS (fingerprints), PIRSF (classification system), SFLD (superfamilies), and NCBIfam. This gives you a unified view of protein domain and family annotations from the world's leading classification resources.

**Q: Can I find which organisms have a specific protein domain?**
Yes. Use the get_entry_taxonomy tool with any InterPro accession to see the taxonomic distribution of that domain or family. This shows which organisms — from bacteria to humans — contain proteins with that specific domain. It is one of the most powerful tools for evolutionary biology, revealing how protein domains have been conserved or diversified across the tree of life.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebi-interpro](https://vinkius.com/mcp/ebi-interpro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EBI InterPro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ebi-interpro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EBI InterPro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebi-interpro": {
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
