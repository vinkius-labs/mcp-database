# PubChem MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubchem)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: Do I need an API key to use PubChem?**
No. PubChem PUG REST is completely free and open without any authentication. The only limitation is a rate limit of 5 requests per second and 400 requests per minute, which is more than sufficient for conversational AI usage.

**Q: What molecular properties are returned for each compound?**
Each compound includes: CID, IUPAC name, molecular formula, molecular weight, canonical SMILES, InChI identifier, XLogP (lipophilicity), hydrogen bond donor count, hydrogen bond acceptor count, and molecular complexity score. These cover Lipinski's Rule of Five for drug-likeness assessment.

**Q: Can I search by molecular formula instead of name?**
Yes! Use the formula search tool with standard notation (e.g., C8H10N4O2 for caffeine, C9H8O4 for aspirin, H2O for water). PubChem will return all compounds matching that exact formula with their names and properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubchem](https://vinkius.com/mcp/pubchem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PubChem** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pubchem` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PubChem** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pubchem": {
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
