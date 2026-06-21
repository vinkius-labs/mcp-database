# Chord Constructor MCP Server

Decompose chord notation into notes, inversions, and harmonic roles.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-constructor)

## Overview
**Category:** productivity
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Chord Constructor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-constructor](https://vinkius.com/mcp/chord-constructor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
