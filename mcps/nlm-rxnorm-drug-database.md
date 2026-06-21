# NLM RxNorm (Drug Database) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nlm-rxnorm-drug-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the NLM RxNorm database to search for drugs, retrieve RxCUIs, and inspect standardized drug properties and identifiers.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NLM RxNorm (Drug Database)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the drug 'Lisinopril' and provide its RxCUI."

**🤖 AI Agent:**
> I found the RxCUI for Lisinopril using `find_rxcui_by_string`. The primary RxCUI is 29046. Would you like to see its detailed properties?

---

**👤 You:**
> "I think I misspelled 'Metformmin'. Can you suggest the correct name?"

**🤖 AI Agent:**
> Using `get_spelling_suggestions`, the closest match for 'Metformmin' is 'Metformin'. I can now search for its properties if you'd like.

---

**👤 You:**
> "Get all properties and attributes for RxCUI 860975."

**🤖 AI Agent:**
> I've retrieved the properties for RxCUI 860975 using `get_all_properties`. This concept refers to 'Aspirin 81 MG Oral Tablet'. It includes attributes from sources like MTHSPL and RXNORM.


## ❓ FAQ

**Q: How can I find the RxCUI for a specific drug name?**
You can use the `find_rxcui_by_string` tool. Simply provide the drug name, and the agent will return the associated RxNorm Concept Unique Identifiers.

**Q: What should I do if I am unsure of the correct spelling of a drug?**
Use the `get_spelling_suggestions` tool. It provides strings similar to your input to help you find the correct standardized drug name.

**Q: Can I retrieve all properties, such as synonyms and attributes, for a drug?**
Yes, the `get_all_properties` tool allows you to fetch detailed attributes, codes, and names associated with a specific RxCUI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nlm-rxnorm-drug-database](https://vinkius.com/mcp/nlm-rxnorm-drug-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NLM RxNorm (Drug Database)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nlm-rxnorm-drug-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NLM RxNorm (Drug Database)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nlm-rxnorm-drug-database": {
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
