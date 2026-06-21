# Fuzzy String Distance Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fuzzy-string-distance-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fuzzy-string-distance-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fuzzy-string-distance-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate exact Levenshtein, Jaro-Winkler, and Dice distances for fuzzy text matching natively local.

## Description
When deduplicating lists of names or correcting misspellings (e.g. 'John Smith' vs 'Jon Smyth'), semantic embeddings are overkill and LLM prompting is unpredictable. This engine provides the academic gold-standard string distances: Levenshtein (edit distance), Jaro-Winkler (prefix-heavy similarity), and Dice coefficient. Computed strictly in local JS, it gives agents a mathematical foundation for entity resolution.


## Available Tools
- **calculate_fuzzy_distance**: Calculates deterministic Levenshtein, Jaro-Winkler, and Dice string distances between two texts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fuzzy String Distance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Jaro-Winkler distance between 'Vinkius' and 'Vinckius'. Is the similarity above 0.9?"

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "What is the exact Levenshtein edit distance between 'kitten' and 'sitting'?"

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Run the fuzzy distance engine on 'Jonathan Doe' and 'Jon Doe'. If Dice coefficient > 0.8, treat them as the same entity."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## Installation & Usage

To install and use the **Fuzzy String Distance Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fuzzy-string-distance-engine](https://vinkius.com/mcp/fuzzy-string-distance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
