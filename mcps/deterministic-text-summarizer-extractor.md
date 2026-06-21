# Deterministic Text Summarizer & Extractor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-text-summarizer-extractor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deterministic-text-summarizer-extractor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deterministic-text-summarizer-extractor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Equip your AI with pure Term Frequency (TF) text analysis. Deterministically extract keywords, bigrams, and generate extractive summaries without external API calls.

## Description
Large Language Models generate 'Abstractive' summaries (they write new text based on their understanding), which consumes a massive amount of tokens and can introduce hallucinations or skip crucial facts. The Text Summarizer & Extractor MCP solves this by using 'Extractive' summarization—a purely mathematical algorithm (Term Frequency) that pulls the exact, unmodified, most important sentences directly from the source text. It is the ultimate pre-processing tool for strict data extraction.

### The Superpowers
- **Extractive Summarization:** Ranks all sentences in a document mathematically by keyword density and extracts the top N sentences. Zero hallucination.
- **Keyword Extraction:** Instantly counts term frequency (TF) to find the most repeated topics, completely ignoring grammatical stop words (English, Portuguese, Spanish).
- **Bigram Analysis:** Finds the most common two-word phrases, perfect for SEO topic modeling and strict semantic analysis.
- **Zero-Dependency Architecture:** Pure Javascript runtime execution guarantees absolute speed without bloated NLP packages.


## Available Tools
- **extract_top_bigrams**: Extracts the top N most frequent two-word phrases (bigrams). Excellent for SEO topic modeling
- **extract_top_keywords**: Extracts the top N most frequent keywords from a text (TF algorithm), ignoring stop words
- **extractive_summary**: Performs algorithmic extractive summarization. It selects the most mathematically important sentences based on Term Frequency (TF)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Text Summarizer & Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 3-sentence extractive summary of this long article."

**🤖 AI Agent:**
> Using the extractive_summary tool (sentenceCount=3): Here are the 3 most mathematically relevant sentences extracted exactly from the source.

---

**👤 You:**
> "What are the top 10 keywords in this SEO text?"

**🤖 AI Agent:**
> Using the extract_top_keywords tool (topN=10): The JSON array shows the top frequency counts, ignoring standard stop words.

---

**👤 You:**
> "Find the top 5 bigrams (two-word phrases) repeated in this transcript."

**🤖 AI Agent:**
> Using the extract_top_bigrams tool: The most repeated bigram is 'machine learning' with 14 occurrences.


## Installation & Usage

To install and use the **Deterministic Text Summarizer & Extractor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-text-summarizer-extractor](https://vinkius.com/mcp/deterministic-text-summarizer-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
