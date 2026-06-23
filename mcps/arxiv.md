# arXiv MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arxiv)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 2.5M+ scientific preprints across physics, computer science, mathematics, biology, economics, and more — with full abstracts, author lists, and direct PDF download links.

## Description
Connect your AI agent to **arXiv** — the world's premier open-access preprint server, operated by Cornell University since 1991. Access cutting-edge research before peer review.

### What you can do

- **Preprint Search** — Find papers by keyword across all scientific domains using relevance ranking. Supports boolean logic and category filtering (cs.AI, cs.LG, physics, math, q-bio, stat, econ)
- **Paper Details** — Get full metadata by arXiv ID: title, all authors, complete abstract, arXiv categories, publication date, DOI (if available), and direct PDF download link

### How it works

1. Subscribe to this server
2. Start searching preprints immediately — no API key required

### Who is this for?

- **AI/ML Engineers** — stay on the cutting edge by searching the latest preprints on transformers, LLMs, reinforcement learning, and diffusion models before they appear in journals
- **Physics Researchers** — access the latest findings in quantum computing, astrophysics, condensed matter, and high-energy physics as they're released
- **Mathematics & Statistics Professionals** — find proofs, new theorems, and statistical methodology papers in real-time


## Available Tools (2)
- **get_arxiv_paper**: IDs look like 2106.09685 or cs/0101001.

Get full preprint details by arXiv ID
- **search_arxiv**: Returns title, authors, abstract, categories, and direct PDF links. Categories: cs.AI, cs.LG, physics, math, q-bio, stat, econ. Perfect for finding cutting-edge research.

Search 2.5M+ scientific preprints across physics, CS, math, biology, and more


## 💬 Prompt Examples

Here are some examples of how you can interact with the **arXiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the latest papers on large language models and reasoning capabilities."

**🤖 AI Agent:**
> Found 10 recent preprints. Highlights: 'Chain-of-Thought Prompting Elicits Reasoning in Large Language Models' (arXiv:2201.11903) by Wei et al. — shows how few-shot CoT prompting enables complex reasoning in LLMs. Categories: cs.CL, cs.AI. Also found: papers on tree-of-thought, self-consistency, and mathematical reasoning. Each with 📥 PDF link.

---

**👤 You:**
> "Get the full details of the 'Attention Is All You Need' paper from arXiv."

**🤖 AI Agent:**
> arXiv:1706.03762 — 'Attention Is All You Need' by Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, Illia Polosukhin. Published: 2017-06-12. Categories: cs.CL, cs.LG. Abstract: The dominant sequence transduction models are based on complex recurrent or convolutional neural networks... We propose a new simple network architecture, the Transformer, based solely on attention mechanisms. 📥 PDF: arxiv.org/pdf/1706.03762

---

**👤 You:**
> "Search arXiv for papers on quantum error correction in the physics category."

**🤖 AI Agent:**
> Found 10 preprints in quant-ph on quantum error correction. Top results: 'Suppressing quantum errors by scaling a surface code logical qubit' — demonstrates below-threshold error rates using Google's Sycamore processor. Also: topological codes, Floquet codes, and bosonic qubit approaches. Each result includes arXiv ID, authors, abstract, and direct PDF link for immediate reading.


## ❓ FAQ

**Q: What is a preprint and how does arXiv work?**
A preprint is a scientific paper shared publicly before formal peer review. arXiv allows researchers to share their findings immediately upon completion, accelerating scientific communication. Papers are assigned a permanent arXiv ID (e.g., 2106.09685) and are freely accessible forever. Many landmark papers in AI, physics, and math appeared on arXiv months or years before journal publication.

**Q: What scientific categories and disciplines does arXiv cover?**
arXiv covers 8 major domains: Physics (astro-ph, cond-mat, hep, quant-ph), Mathematics (math.*), Computer Science (cs.AI, cs.LG, cs.CL, cs.CV, cs.CR, etc.), Quantitative Biology (q-bio), Quantitative Finance (q-fin), Statistics (stat), Electrical Engineering (eess), and Economics (econ). Each domain has multiple sub-categories for precise filtering.

**Q: Is arXiv free and do I need an API key?**
Yes, arXiv is completely free and operated as a non-profit by Cornell University. No API key or registration is required for search queries. The only limitation is a rate limit of approximately 1 request per 3 seconds for the search API. All papers are freely downloadable as PDF and accessible in perpetuity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arxiv](https://vinkius.com/mcp/arxiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **arXiv** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arxiv` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **arXiv** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arxiv": {
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
