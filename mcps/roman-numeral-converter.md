# Roman Numeral Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roman-numeral-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/roman-numeral-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/roman-numeral-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert musical chord names to Roman numerals and vice-versa, with automatic transposition.

## Description
The Roman Numeral Converter MCP allows musicians and theorists to bridge the gap between note-based progressions and functional harmonic notation. Using tools like `parse_progression_string`, `resolve_harmonic_function`, `transpose_progression`, and `get_chord_metadata`, you can instantly transform a sequence of chords (e.g., C-Am-F-G) into its Roman numeral equivalent (I-vi-IV-V). The server also supports automatic transposition, allowing you to shift any progression to a new target key while preserving the underlying harmonic functions and scale degrees.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roman Numeral Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this progression: C-Am-F-G"

**🤖 AI Agent:**
> The parsed chords are: C, Am, F, G.

---

**👤 You:**
> "What is the harmonic function of Am in the key of C?"

**🤖 AI Agent:**
> In the key of C, Am is the vi (minor) degree, which you can find using `resolve_harmonic_function`.

---

**👤 You:**
> "Transpose I-vi-IV-V from C to G."

**🤖 AI Agent:**
> The transposed progression in G is: G, Em, C, D, calculated via `transpose_progression`.


## Installation & Usage

To install and use the **Roman Numeral Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roman-numeral-converter](https://vinkius.com/mcp/roman-numeral-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
