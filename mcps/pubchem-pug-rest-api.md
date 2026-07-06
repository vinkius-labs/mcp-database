# PubChem PUG REST API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubchem-pug-rest-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access chemical data — audit compounds, formulas, and CIDs via AI.

## Description
Empower your AI agent to orchestrate your entire chemical research and compound auditing workflow with the **PubChem PUG REST API**, the authoritative source for molecular data from the National Library of Medicine. By connecting PubChem to your agent, you transform complex chemical searches into a natural conversation. Your agent can instantly retrieve compound details, audit molecular formulas, and query specific Compound Identifiers (CIDs) without you ever touching a scientific portal. Whether you are conducting pharmacological research or managing laboratory constraints, your agent acts as a real-time chemical consultant, ensuring your data is always verified and precise.

### What you can do

- **Compound Auditing** — Search for thousands of chemical compounds by name or keyword and retrieve detailed metadata, including IUPAC names and formulas.
- **CID Oversight** — Audit specific Compound Identifiers (CIDs) to understand the technical reach of your chemical data instantly.
- **Formula Discovery** — Query molecular formulas for specific compounds to assist in deep-dive archival classification.
- **Metadata Intelligence** — Retrieve high-resolution technical properties for any chemical record to assist in scientific auditing.
- **Operational Monitoring** — Check API status to ensure your chemical research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (PubChem is a free and open service)
3. Start managing your chemical intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Scientists & Researchers** — monitor chemical data and retrieve official metadata straight from your workflow.
- **Pharmacologists** — verify compound details and audit molecular patterns without manual searching.
- **Students & Educators** — perform rapid audits of chemical properties and identify relevant stylistic markers through natural language.
- **Operations Leads** — automate scientific data querying to orchestrate cross-functional research teams smoothly.


## Available Tools (4)
- **get_compound_by_name**: Get comprehensive details for a chemical compound by name
- **search_compound_cids**: Search for compound CIDs matching a name or keyword
- **check_api_status**: Check if the PubChem PUG REST service is operational
- **get_compound_by_cid**: Get comprehensive details for a chemical compound by CID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubChem PUG REST API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for compound 'Aspirin' using PubChem."

**🤖 AI Agent:**
> I've retrieved the details for Aspirin! It has a CID of 2244 and its molecular formula is identified as C9H8O4. Would you like the full IUPAC name or other technical metadata for this compound?

---

**👤 You:**
> "What is the molecular formula for CID '2519'?"

**🤖 AI Agent:**
> I've identified the compound for CID 2519! It is Caffeine, and its molecular formula is identified as C8H10N4O2. I can assist you with more technical properties for this record if you'd like.

---

**👤 You:**
> "Search for compound CIDs matching 'glucose'."

**🤖 AI Agent:**
> I've scanned the PubChem database for glucose! I've identified several matching CIDs, including 5793 and 107526. I can provide the full metadata for any of these identifiers to help you in your research.


## ❓ FAQ

**Q: Is an API Key required for PubChem API?**
No. PubChem is a free and open service provided by the NIH. This server works out of the box without any static credentials required.

**Q: What is a CID?**
CID stands for Compound Identifier. It is a unique numerical ID assigned to each chemical compound in the PubChem database.

**Q: Can the agent show molecular formulas?**
Yes. The compound details retrieved by your agent include the molecular formula and IUPAC name metadata where available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubchem-pug-rest-api](https://vinkius.com/mcp/pubchem-pug-rest-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PubChem PUG REST API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pubchem-pug-rest-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PubChem PUG REST API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pubchem-pug-rest-api": {
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
