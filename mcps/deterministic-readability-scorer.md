# Deterministic Readability Scorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-readability-scorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deterministic-readability-scorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deterministic-readability-scorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI with strict linguistic math. Calculate Flesch-Kincaid, Gunning Fog indexes, and exact reading times deterministically.

## Description
AI models perceive text as 'tokens', not as phonetic syllables or strict sentence boundaries. Because of this, asking an LLM to calculate a Flesch-Kincaid readability score directly will always result in a mathematical hallucination. The Readability Scorer MCP solves this by routing text analysis through a deterministic V8 Javascript engine.

### The Superpowers
- **Flesch-Kincaid Precision:** Automatically extracts total syllables, words, and sentences to provide mathematically perfect Reading Ease and Grade Level scores.
- **Gunning Fog Index:** Determines the complexity of your text by algorithmically scanning for polysyllabic words (3+ syllables).
- **Exact Reading Time:** Instead of guessing, it calculates the exact chronological reading time (minutes and seconds) based on a configurable WPM (Words Per Minute).
- **Zero-Dependency Architecture:** Pure Javascript runtime execution means absolute processing speed with no external bloated packages.


## Available Tools
- **calculate_flesch_kincaid**: Provide the full text string.

Analyzes text readability using the deterministic Flesch-Kincaid algorithm
- **calculate_gunning_fog**: Provide the full text string.

Analyzes text readability using the deterministic Gunning Fog index algorithm
- **calculate_reading_time**: Provide the text and optionally the Words Per Minute (WPM) speed (defaults to 200).

Provides an exact reading time estimation based on word count and WPM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Readability Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Flesch-Kincaid Grade Level of my latest blog post?"

**🤖 AI Agent:**
> Using the calculate_flesch_kincaid tool: The text scores a Grade Level of 8.4, meaning it's highly readable for average audiences.

---

**👤 You:**
> "How many minutes will it take a user to read this newsletter?"

**🤖 AI Agent:**
> Using the estimate_reading_time tool (wpm=220): It will take exactly 3 min 15 sec.

---

**👤 You:**
> "Analyze this legal contract using the Gunning Fog Index."

**🤖 AI Agent:**
> Using the calculate_gunning_fog tool: The index is 16.2 due to a high volume of complex, poly-syllabic words.


## Installation & Usage

To install and use the **Deterministic Readability Scorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-readability-scorer](https://vinkius.com/mcp/deterministic-readability-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
