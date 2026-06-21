# Chord Progression Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-progression-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze chord sequences to identify Roman numeral functions, harmonic patterns, and emotional context.

## Description
The Chord Progression Analyzer is a specialized tool for musicians and music theorists. It bridges the gap between raw chord sequences and deep harmonic understanding. By using tools like `analyze_roman_numerals`, you can convert any list of chords into their Roman numeral functions relative to a specific key. The system also features `classify_progression` to detect complex patterns such as cadences or secondary dominants, and `lookup_musical_context` to reveal the emotional resonance and common musical genres associated with those specific movements. This MCP server is ideal for use in Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (3)
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


## ❓ FAQ

**Q: What can I analyze with this tool?**
You can provide a sequence of chords and a key to find their Roman numeral functions using `analyze_roman_numerals`, identify harmonic patterns with `classify_progression`, and discover the emotional impact of those patterns via `lookup_musical_context`.

**Q: How do I specify the key?**
When using `analyze_roman_numerals`, provide the tonality as a string, for example, 'C Major' or 'A Minor'.

**Q: Does it support different musical genres?**
Yes, the `lookup_musical_context` tool provides information on which musical genres frequently utilize specific harmonic progressions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-progression-analyzer](https://vinkius.com/mcp/chord-progression-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chord Progression Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chord-progression-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chord Progression Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chord-progression-analyzer": {
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
