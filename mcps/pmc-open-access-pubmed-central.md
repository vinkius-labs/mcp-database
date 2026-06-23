# PMC Open Access (PubMed Central) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pmc-open-access-pubmed-central)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of open-access biomedical and life sciences research articles. Search metadata, convert IDs, and discover full-text resources.

## Description
Connect to the **PubMed Central (PMC) Open Access Subset** to empower your AI agent with direct access to millions of peer-reviewed biomedical research articles. This server provides comprehensive tools for literature discovery, metadata harvesting, and identifier management.

### What you can do

- **Metadata Harvesting** — Use OAI-PMH protocols to list identifiers, metadata formats, and full records from the PMC repository.
- **Identifier Conversion** — Seamlessly translate between PMCIDs, PMIDs, DOIs, and Manuscript IDs using the official PMC ID Converter.
- **Resource Discovery** — Locate downloadable PDF, XML, and TGZ files for open-access articles to facilitate deep analysis.
- **Citation Export** — Retrieve formatted citations for PubMed and PMC records to streamline academic writing and referencing.
- **Deep Record Inspection** — Fetch specific article metadata or full-text records using unique OAI identifiers.

### How it works

1. Subscribe to this server
2. Provide your NCBI API Key (Tool Name) and registered email
3. Start querying the world's largest repository of life sciences literature directly from your AI client

### Who is this for?

- **Researchers & Academics** — Automate literature reviews, find full-text sources, and manage citations without manual searching.
- **Data Scientists** — Harvest large-scale biomedical datasets for NLP, trend analysis, or knowledge graph construction.
- **Medical Professionals** — Quickly find peer-reviewed evidence and convert clinical identifiers into accessible research papers.


## Available Tools (8)
- **convert_ids**: Returns JSON.

Convert between PMCIDs, PMIDs, DOIs, and Manuscript IDs
- **export_citation**: Export formatted citations for PubMed and PMC articles
- **oa_discover**: ) for PMC articles.

Discover downloadable resources from the PMC Open Access Subset
- **oai_get_record**: Get a specific OAI record from PMC
- **oai_identify**: Identify the PMC OAI-PMH repository
- **oai_list_identifiers**: Use metadataPrefix (e.g., pmc, pmc_fm, oai_dc).

List OAI identifiers for PMC articles
- **oai_list_metadata_formats**: Optionally filter by a specific identifier.

List available metadata formats in PMC OAI-PMH
- **oai_list_records**: List full OAI records for PMC articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PMC Open Access (PubMed Central)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the following PMIDs to PMCIDs: 34567890, 34567891."

**🤖 AI Agent:**
> I've converted those IDs for you. PMID 34567890 corresponds to PMCID PMC8451234 and DOI 10.1038/s41586-021-03850-x.

---

**👤 You:**
> "Find the PDF download link for PMCID PMC5334499."

**🤖 AI Agent:**
> I found the resources for PMC5334499. You can download the PDF directly from the PMC Open Access archive at the following URL: [URL].

---

**👤 You:**
> "List the metadata formats supported by the PMC OAI-PMH repository."

**🤖 AI Agent:**
> The PMC repository supports several metadata formats, including 'oai_dc' (Dublin Core), 'pmc' (Full-text XML), and 'pmc_fm' (Front matter only).


## ❓ FAQ

**Q: How can I find the DOI or PMID for a specific PMCID?**
Use the `convert_ids` tool. Simply provide the PMCID (e.g., PMC5334499) and it will return the corresponding PMID, DOI, and other associated identifiers.

**Q: Can I get direct download links for research papers?**
Yes! The `oa_discover` tool allows you to find downloadable resources like PDFs or XML files for articles in the PMC Open Access Subset using their PMCID.

**Q: How do I retrieve the full metadata for a specific article?**
Use the `oai_get_record` tool with the article's OAI identifier and a metadata prefix like 'pmc' or 'oai_dc' to fetch the complete record details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pmc-open-access-pubmed-central](https://vinkius.com/mcp/pmc-open-access-pubmed-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PMC Open Access (PubMed Central)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pmc-open-access-pubmed-central` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PMC Open Access (PubMed Central)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pmc-open-access-pubmed-central": {
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
