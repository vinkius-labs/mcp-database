# Deterministic Readability Scorer MCP Server

Equip your AI with strict linguistic math. Calculate Flesch-Kincaid, Gunning Fog indexes, and exact reading times deterministically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-readability-scorer)

## Overview
**Category:** productivity
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Deterministic Readability Scorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-readability-scorer](https://vinkius.com/mcp/deterministic-readability-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
