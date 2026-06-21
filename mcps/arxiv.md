# arXiv MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arxiv)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arxiv-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arxiv-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **arXiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arxiv](https://vinkius.com/mcp/arxiv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
