# Chord Substitution Finder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-substitution-finder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chord-substitution-finder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chord-substitution-finder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [music-theory](../categories/music-theory.md)

Identify harmonic substitutions and analyze tension in chord progressions.

## Description
The Chord Substitution Finder is a music theory engine that identifies various substitution patterns for single chords or entire progressions. Using tools like `find_substitutions`, `analyze_progression_tension`, and `get_substitution_detail`, you can explore Tritone, Relative, Parallel, Diatonic, and Chromatic Mediant substitutions. The engine evaluates how each change affects harmonic tension and voice leading motion, providing a deep analysis of musical movement.


## Available Tools
- **analyze_progression_tension**: Analyze the tension arc of a chord progression
- **get_substitution_detail**: Get detailed information about a specific chord substitution
- **find_substitutions**: Find available chord substitutions for a given chord


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chord Substitution Finder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find substitutions for G7."

**🤖 AI Agent:**
> Running `find_substitutions` for G7... Found Tritone substitution: Db7, which increases tension and creates chromatic movement.

---

**👤 You:**
> "Analyze the tension of [Cmaj7, Am7, Dm7, G7]."

**🤖 AI Agent:**
> Using `analyze_progression_tension`... The progression starts with Low tension (Cmaj7) and moves through Medium tension to a High tension dominant (G7).

---

**👤 You:**
> "What is a Tritone substitution?"

**🤖 AI Agent:**
> According to `get_substitution_detail`, a Tritone substitution replaces a dominant seventh chord with another dominant seventh chord an augmented fourth away.


## Installation & Usage

To install and use the **Chord Substitution Finder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-substitution-finder](https://vinkius.com/mcp/chord-substitution-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
