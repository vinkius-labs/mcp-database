# Semantic Scholar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semantic-scholar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 200M+ academic papers with AI-powered TLDR summaries, influential citation tracking, and researcher profiles from the Allen Institute for AI.

## Description
Connect your AI agent to the **world's most AI-enhanced academic knowledge graph**, built and maintained by the Allen Institute for AI (AI2).

### What you can do

- **AI-Powered Search** — Find papers across 200M+ works with AI-generated TLDR summaries that distill each paper into a single sentence of key insight
- **Influential Citations** — Beyond simple citation count, see how many *influential* citations a paper has received — those that meaningfully build upon the cited work
- **Multi-Format Lookup** — Access papers by Semantic Scholar ID, DOI, ArXiv ID (arXiv:2106.09685), or PubMed ID (PMID:12345)
- **Citation Graph** — Explore the full citation chain of any paper, with TLDR summaries for each citing work
- **Researcher Profiles** — Find academics by name with paper counts, total citations, and h-index metrics

### How it works

1. Subscribe to this server
2. Start searching 200M+ papers immediately — no API key required for basic usage

### Who is this for?

- **AI/ML Researchers** — find relevant papers in your field with instant TLDR summaries to quickly assess relevance before reading the full text
- **Graduate Students** — build comprehensive literature reviews using the citation graph to trace how ideas evolve across the academic landscape
- **R&D Teams** — evaluate researcher impact using influential citation counts and h-index metrics for talent scouting or collaboration decisions


## Available Tools (4)
- **get_semantic_citations**: Essential for literature reviews and impact analysis.

Find papers that cite a specific work on Semantic Scholar
- **get_semantic_paper**: Accepts Semantic Scholar paper ID, DOI, ArXiv ID (e.g. arXiv:2106.09685), or PMID (e.g. PMID:12345).

Get full paper details from Semantic Scholar by paper ID or DOI
- **search_semantic_author**: Returns paper count, total citations, and h-index for each researcher.

Find researchers and their publication metrics on Semantic Scholar
- **search_semantic_scholar**: Returns papers with AI-generated TLDR summaries, citation counts, influential citation counts, and fields of study. Covers Computer Science, Medicine, Biology, Physics, and all STEM fields.

Search 200M+ academic papers with AI-powered TLDR summaries and influence scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Semantic Scholar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most cited papers on transformer architecture in deep learning?"

**🤖 AI Agent:**
> Top results include: 'Attention Is All You Need' by Vaswani et al. (2017) — 🤖 TLDR: The Transformer, a new network architecture based solely on attention mechanisms, achieves superior quality on machine translation tasks. Cited 120,000+ times (25,000+ influential). Fields: Computer Science, Linguistics.

---

**👤 You:**
> "Get the full details of the LoRA paper using its ArXiv ID arXiv:2106.09685."

**🤖 AI Agent:**
> Found: 'LoRA: Low-Rank Adaptation of Large Language Models' by Edward Hu et al. (2021). 🤖 TLDR: LoRA freezes the pre-trained model weights and injects trainable rank decomposition matrices, reducing trainable parameters by 10,000x and GPU memory by 3x. Citations: 8,500+ (2,100 influential). Fields: CS, Mathematics. Available at arxiv.org/abs/2106.09685.

---

**👤 You:**
> "Find the researcher Yann LeCun and show me his publication metrics."

**🤖 AI Agent:**
> Found researcher Yann LeCun — Author at Meta AI / NYU. Papers: 950+, Total Citations: 380,000+, h-index: 162. Known for pioneering work in convolutional neural networks, self-supervised learning, and modern AI architectures. Profile link and full publication list available.


## ❓ FAQ

**Q: Do I need an API key to use Semantic Scholar?**
No API key is required for basic usage. The public API provides 5,000 requests per 5 minutes shared among unauthenticated users. For higher throughput, academic and institutional users can request a free API key at semanticscholar.org, which grants dedicated rate limits of 1–10 requests per second depending on the endpoint.

**Q: What is the TLDR feature and how does it work?**
TLDR (Too Long; Didn't Read) is an AI-generated one-sentence summary of each paper, powered by Allen AI's SciTLDR NLP model. It distills the key contribution or finding of a paper into a single, easily digestible sentence — ideal for quickly scanning relevance without reading an entire abstract or paper.

**Q: What is the difference between total citations and influential citations?**
Total citations count every paper that references the work. Influential citations are a subset — papers where the cited work meaningfully contributes to the citing paper's research (not just a passing mention in the related work section). This metric is calculated by Semantic Scholar's AI models and provides a much more accurate measure of real scientific impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semantic-scholar](https://vinkius.com/mcp/semantic-scholar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Semantic Scholar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `semantic-scholar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Semantic Scholar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semantic-scholar": {
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
