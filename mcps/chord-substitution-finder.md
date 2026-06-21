# Chord Substitution Finder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chord-substitution-finder)
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


## ❓ FAQ

**Q: What types of substitutions can I find?**
The engine supports Tritone, Relative, Parallel, Diatonic, and Chromatic Mediant substitutions.

**Q: How do I analyze a whole progression?**
Use the `analyze_progression_tension` tool by providing a JSON array of chords.

**Q: Can I see how voice leading changes?**
Yes, the `find_substitutions` tool provides details on the voice leading effect for each substitution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chord-substitution-finder](https://vinkius.com/mcp/chord-substitution-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chord Substitution Finder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chord-substitution-finder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chord Substitution Finder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chord-substitution-finder": {
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
