# Chord Constructor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-constructor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chord-constructor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chord-constructor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Decompose chord notation into notes, inversions, and harmonic roles.

## Description
The Chord Constructor MCP server is a powerful musical engine that allows AI agents to analyze complex chord structures. By using tools like `parse_chord_string`, you can break down any notation into its constituent intervals and roots. The server also provides advanced music theory capabilities, such as calculating all possible inversions with `get_chord_inversions`, generating specific textures via `generate_voicings` (supporting both closed and open styles), and identifying the functional role of a chord in a key using `determine_harmonic_role`. This makes it an essential tool for music composition, theory analysis, and automated arrangement tasks.


## Available Tools
- **determine_harmonic_role**: Identifies the functional role of a chord within a specific musical key
- **generate_voicings**: Returns both voicings.

Arranges a set of notes into specific "closed" or "open" musical textures
- **get_chord_inversions**: Returns inversions with bassNote and fullStack.

Calculates all possible permutations of a chord where different notes serve as the bass
- **parse_chord_string**: Returns root, intervals, and normalized name.

Converts a standard chord name string into its structured component parts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chord Constructor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse the chord 'Ebmaj7'."

**🤖 AI Agent:**
> The `parse_chord_string` tool identifies the root as Eb and the intervals as major third, perfect fifth, and minor seventh.

---

**👤 You:**
> "What are the inversions for the notes [C, E, G]?"

**🤖 AI Agent:**
> Using `get_chord_inversions`, you can find all three permutations: root position (C-E-G), first inversion (E-G-C), and second inversion (G-C-E).

---

**👤 You:**
> "Generate an open voicing for [C, E, G, B]."

**🤖 AI Agent:**
> The `generate_voicings` tool produces an expanded arrangement of the notes to create more space in the sound.


## Installation & Usage

To install and use the **Chord Constructor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-constructor](https://vinkius.com/mcp/chord-constructor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
