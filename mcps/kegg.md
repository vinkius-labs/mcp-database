# KEGG MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kegg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the Kyoto Encyclopedia of Genes and Genomes (KEGG) to query genomic, chemical, and systemic functional information directly from your AI agent.

## Description
Connect your AI agent to the **KEGG** (Kyoto Encyclopedia of Genes and Genomes) database, the gold standard for bioinformatics and systems biology. This server enables deep exploration of biological pathways, genomes, and chemical substances through natural language.

### What you can do

- **Genomic Exploration** — Retrieve detailed information about genes, proteins, and organisms using `kegg_get` and `kegg_list`.
- **Pathway Analysis** — Map genes to metabolic or signaling pathways and visualize biological systems using `kegg_link`.
- **Chemical & Drug Data** — Search for compounds, glycans, and drugs by keyword, formula, or mass using `kegg_find`.
- **Drug Interactions** — Identify adverse drug-drug interactions (DDI) specifically for clinical and pharmacological research via `kegg_ddi`.
- **Identifier Conversion** — Seamlessly convert between KEGG IDs and outside databases like NCBI, UniProt, and PubChem using `kegg_conv`.

### How it works

1. Subscribe to this server
2. Configure your access credentials (if required by your proxy)
3. Start querying biological data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bioinformatics Researchers** — automate the retrieval of gene sequences and pathway maps without manual REST calls.
- **Pharmacologists** — quickly check drug-drug interactions and chemical properties during drug discovery workflows.
- **Data Scientists** — integrate high-quality biological metadata into analysis pipelines directly from the chat interface.


## Available Tools (7)
- **kegg_info**: g., kegg, pathway, brite, genes, hsa, compound).

Displays database release information and statistics
- **kegg_link**: g., pathways linked from human genes).

Finds related entries using database cross-references
- **kegg_list**: For pathway/brite, can specify organism/option. Use "organism" to list all KEGG organisms.

Obtains a list of entry identifiers and associated names
- **kegg_conv**: Converts KEGG identifiers to/from outside identifiers
- **kegg_ddi**: Finds adverse drug-drug interactions
- **kegg_find**: Finds entries matching a query keyword or chemical data
- **kegg_get**: g., hsa:10458+ece:Z5100).

Retrieves database entries in flat-file or specific file formats


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KEGG** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available organisms in the KEGG database."

**🤖 AI Agent:**
> I'll use `kegg_list` with the 'organism' parameter. I've found thousands of entries, including 'hsa' (Homo sapiens), 'mmu' (Mus musculus), and 'eco' (Escherichia coli). Which one would you like to explore?

---

**👤 You:**
> "Search for compounds with the keyword 'glucose' in the KEGG database."

**🤖 AI Agent:**
> Running `kegg_find` for 'glucose' in the compound database... I found several entries, including C00031 (D-Glucose) and C00221 (beta-D-Glucose). Would you like the full details for C00031?

---

**👤 You:**
> "Get the full entry details for the human gene hsa:10458."

**🤖 AI Agent:**
> Fetching data using `kegg_get` for 'hsa:10458'... This gene corresponds to ACSL4 (acyl-CoA synthetase long chain family member 4). It is involved in metabolic pathways like Fatty acid metabolism (hsa00071).


## ❓ FAQ

**Q: How can I find all metabolic pathways associated with a specific human gene?**
You can use the `kegg_link` tool. Specify 'pathway' as the target_db and the human gene ID (e.g., 'hsa:10458') as the source_db to retrieve all linked biological pathways.

**Q: Can I search for chemical compounds using an exact molecular mass?**
Yes! Use the `kegg_find` tool with the database set to 'compound', the mass value as the query, and the option set to 'exact_mass'.

**Q: Is it possible to check for interactions between multiple drugs at once?**
Absolutely. Use the `kegg_ddi` tool and provide the drug identifiers separated by a '+' sign (e.g., 'D00564+D00017') to find known adverse interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kegg](https://vinkius.com/mcp/kegg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KEGG** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kegg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KEGG** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kegg": {
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
