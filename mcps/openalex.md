# OpenAlex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openalex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access 250M+ scholarly works with open bibliometric data — search papers, authors, institutions, and trending research topics. The open-source alternative to Scopus and Web of Science.

## Description
Connect your AI agent to the **world's largest fully open catalog of scholarly works** — a free, CC0-licensed replacement for enterprise platforms like Scopus and Web of Science.

### What you can do

- **Works Search** — Search 250M+ works with complete metadata including authors, institutional affiliations, citation counts, open access status, and reconstructed abstracts
- **Author Profiles** — Find researchers worldwide with publication counts, total citations, h-index metrics, and current institutional affiliation
- **Institution Discovery** — Explore the research output of universities, labs, hospitals, and government agencies globally with full bibliometric data
- **Research Trends** — Discover the most researched scientific topics ranked by total number of published works to understand where the scientific community is focusing
- **Open Access Detection** — Every work indicates its open access status (green, gold, hybrid, bronze) for instant full-text availability assessment

### How it works

1. Subscribe to this server
2. Enter your OpenAlex API key (free — create an account at openalex.org)
3. Start exploring 250M+ scholarly works from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Academic Researchers** — run comprehensive bibliometric analyses without expensive Scopus or Web of Science subscriptions
- **University Librarians** — monitor institutional research output, track citation metrics, and identify collaboration opportunities
- **Science Policy Analysts** — analyze global research trends, funding impacts, and institutional performance across countries and disciplines


## Available Tools (5)
- **get_openalex_trending_topics**: Essential for understanding global research trends.

Discover the most researched scientific topics and concepts globally
- **get_openalex_work**: Accepts OpenAlex ID (e.g. W2741809809 or full URL) or DOI (e.g. 10.1038/nature12373).

Get full details of an academic work by OpenAlex ID or DOI
- **search_openalex_authors**: Returns works count, total citations, h-index, current institution, and top research concepts.

Find researchers with publication metrics, h-index, and institutional affiliations
- **search_openalex_institutions**: Returns publication counts, citation metrics, country, and top research areas. Covers universities, research labs, hospitals, and government agencies globally.

Find research institutions, universities, and organizations worldwide
- **search_openalex_works**: Returns title, authors with institutional affiliations, journal, year, citation count, open access status, concepts, and reconstructed abstracts. CC0 licensed data.

Search 250M+ academic works in the world's largest open scholarly database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAlex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which institutions publish the most research on quantum computing worldwide?"

**🤖 AI Agent:**
> Top institutions for quantum computing: MIT (2,400+ works, 180K citations), Stanford University (1,800+ works), University of Waterloo (1,500+ works), ETH Zurich (1,200+ works), and Google DeepMind (800+ works). Each result includes citation metrics, country code, and top research concepts.

---

**👤 You:**
> "Search for Geoffrey Hinton and show me his publication metrics and affiliations."

**🤖 AI Agent:**
> Found: Geoffrey Hinton — University of Toronto / Google Brain. Works: 650+, Citations: 750,000+, h-index: 183. Top concepts: Machine Learning, Neural Networks, Deep Learning, Artificial Intelligence. His most cited work: 'ImageNet Classification with Deep Convolutional Neural Networks' (2012) with 120,000+ citations.

---

**👤 You:**
> "What are the most researched scientific topics globally right now?"

**🤖 AI Agent:**
> Top 5 research topics by published works: 1) Medicine (45M+ works, 1.2B citations), 2) Biology (35M+ works), 3) Chemistry (30M+ works), 4) Computer Science (20M+ works), 5) Physics (18M+ works). At the granular level, trending sub-topics include: Large Language Models, mRNA therapeutics, CRISPR applications, and climate modeling.


## ❓ FAQ

**Q: Is the OpenAlex API key free and how do I get one?**
Yes, the API key is completely free. OpenAlex provides 100,000 credits per day at no cost. Create your free account at openalex.org, then navigate to Settings → API to generate your key. The key is required since February 2026 when OpenAlex retired the 'polite pool' system.

**Q: How does OpenAlex compare to Scopus and Web of Science?**
OpenAlex is a fully open, CC0-licensed alternative covering 250M+ works — comparable in scope to Scopus (90M+) and far exceeding Web of Science (90M+). It provides citation metrics, h-indexes, institutional data, and open access detection. The key difference: OpenAlex is completely free with no institutional subscription required, while Scopus and WoS cost thousands of dollars per year.

**Q: What data is available for each scholarly work?**
Each work includes: title, authors with institutional affiliations, publication year, journal/source, DOI, work type, citation count, open access status and URL, research topics/concepts, and a reconstructed abstract. Author profiles add h-index, total publications, and career affiliations. Institutions include country, type, and research area specializations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openalex](https://vinkius.com/mcp/openalex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenAlex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openalex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenAlex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openalex": {
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
