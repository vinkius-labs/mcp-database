# CrossRef MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crossref)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 140M+ scholarly works across all scientific disciplines — with DOI resolution, citation counts, author lookup, and full bibliographic metadata from the world's largest DOI registry.

## Description
Give your AI agent direct access to the **world's largest registry of scholarly metadata** — 140M+ records spanning every DOI ever assigned across all scientific publishers.

### What you can do

- **Universal Search** — Find any published work across journals, books, conference papers, datasets, and dissertations using free-text queries
- **DOI Resolution** — Instant metadata lookup for any DOI with title, complete author list, journal, year, type, and citation count
- **Author Discovery** — Search for all publications by a specific researcher name across all major publishers simultaneously

### How it works

1. Subscribe to this server
2. Start resolving DOIs and searching scholarly works immediately — no API key required

### Who is this for?

- **Academic Researchers** — resolve DOIs, verify citations, and build comprehensive bibliographies without leaving their AI assistant
- **Science Writers** — instantly retrieve publication details to verify facts and cite sources accurately
- **Data Analysts** — explore the scholarly landscape with citation metrics and publisher data for bibliometric analysis


## Available Tools (3)
- **get_crossref_doi**: g. 10.1038/nature12373) and get complete metadata: title, all authors, journal, year, type, citation count, and abstract.

Look up any scholarly work by its DOI
- **search_crossref_author**: Returns their publications sorted by relevance with citation counts.

Find publications by a specific author
- **search_crossref**: Every result includes DOI, citation count, and full bibliographic data. The world's largest DOI registry.

Search 140M+ scholarly works across all scientific disciplines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrossRef** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up the paper with DOI 10.1038/nature12373 and show me all its details."

**🤖 AI Agent:**
> Found: 'Sequence-specific antimicrobials using efficiently delivered RNA-guided nucleases' by David Bikard et al. Published in Nature Biotechnology (2014). Type: journal-article. Cited 682 times. This is a pioneering paper on using CRISPR-Cas9 for targeted antimicrobial applications. DOI resolves to the publisher page for full-text access.

---

**👤 You:**
> "Find all publications by Jennifer Doudna related to gene editing."

**🤖 AI Agent:**
> Found 10 works by Jennifer Doudna. Top results include her landmark 2012 Science paper 'A Programmable Dual-RNA-Guided DNA Endonuclease in Adaptive Bacterial Immunity' (cited 15,000+ times), follow-up work on CRISPR applications in Nature, and reviews in Cell. Each entry includes DOI, journal, year, and full citation count.

---

**👤 You:**
> "Search CrossRef for the latest research on quantum computing error correction."

**🤖 AI Agent:**
> Found 10 relevant works. Highlights: 'Suppressing quantum errors by scaling a surface code logical qubit' in Nature (2023) — cited 320 times. Also found recent work from Google Quantum AI and IBM Research on topological error correction codes. All results include DOI, full author lists, and citation metrics.


## ❓ FAQ

**Q: What exactly is a DOI and why is CrossRef important?**
A Digital Object Identifier (DOI) is a unique, permanent identifier assigned to every published scholarly work — like a social security number for academic papers. CrossRef maintains the world's largest DOI registry with 140M+ records, making it the authoritative source for bibliographic metadata across all publishers globally.

**Q: Is authentication or registration required to use this server?**
No. CrossRef's public API is free and open without authentication. Adding a polite email in the User-Agent header (which this server does automatically) grants access to the 'polite pool' with significantly faster response times.

**Q: What types of scholarly works can I find through CrossRef?**
CrossRef covers virtually every type of scholarly output: journal articles, book chapters, conference proceedings, preprints, datasets, dissertations, and technical reports. It aggregates metadata from 20,000+ publishers including Elsevier, Springer Nature, Wiley, Oxford University Press, and thousands of smaller publishers worldwide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crossref](https://vinkius.com/mcp/crossref)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrossRef** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crossref` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrossRef** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crossref": {
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
