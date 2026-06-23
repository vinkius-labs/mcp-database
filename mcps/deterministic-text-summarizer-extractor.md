# Deterministic Text Summarizer & Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-text-summarizer-extractor)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: What is the difference between Extractive and Abstractive summarization?**
Abstractive summarization (what ChatGPT does) writes a completely new text based on its understanding. Extractive summarization (what this tool does) selects the most mathematically important sentences directly from the original text without changing a single word. It guarantees 100% factual accuracy.

**Q: Does the keyword extraction ignore simple connection words?**
Yes. It has a built-in cross-language 'Stop Words' dictionary (supporting English, Portuguese, and Spanish) to ensure words like 'the', 'and', 'for', 'uma' are completely ignored during Term Frequency calculations.

**Q: Why use this tool instead of just asking an AI to summarize?**
If you have a massive 50-page document, passing the entire text into an AI context window is extremely expensive and slow. Running an algorithmic extraction first condenses the text dramatically while retaining all key facts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-text-summarizer-extractor](https://vinkius.com/mcp/deterministic-text-summarizer-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Text Summarizer & Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-text-summarizer-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Text Summarizer & Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-text-summarizer-extractor": {
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
