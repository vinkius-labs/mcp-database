# Chord Progression Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-progression-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chord-progression-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chord-progression-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze chord sequences to identify Roman numeral functions, harmonic patterns, and emotional context.

## Description
The Chord Progression Analyzer is a specialized tool for musicians and music theorists. It bridges the gap between raw chord sequences and deep harmonic understanding. By using tools like `analyze_roman_numerals`, you can convert any list of chords into their Roman numeral functions relative to a specific key. The system also features `classify_progression` to detect complex patterns such as cadences or secondary dominants, and `lookup_musical_context` to reveal the emotional resonance and common musical genres associated with those specific movements. This MCP server is ideal for use in Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools
- **analyze_roman_numerals**: g., "C Major") and returns the scale degrees as Roman numerals.

Converts a list of named chords into their corresponding Roman numeral functions relative to a provided key
- **classify_progression**: Analyzes a sequence of Roman numerals to identify the overarching harmonic pattern
- **lookup_musical_context**: Retrieves the stylistic and emotional metadata associated with a specific progression type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chord Progression Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the progression C, Am, F, G in the key of C Major."

**🤖 AI Agent:**
> The Roman numeral functions for this sequence are ["I", "vi", "IV", "V"].

---

**👤 You:**
> "What is the harmonic pattern of ['I', 'IV', 'V', 'I']?"

**🤖 AI Agent:**
> The identified progression type is a cadence.

---

**👤 You:**
> "What emotion is associated with a 'secondary dominant'?"

**🤖 AI Agent:**
> A secondary dominant typically evokes tension and movement.


## Installation & Usage

To install and use the **Chord Progression Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-progression-analyzer](https://vinkius.com/mcp/chord-progression-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
