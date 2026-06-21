# Roman Numeral Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roman-numeral-converter)
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


## ❓ FAQ

**Q: What can this tool do?**
It parses chord progressions, identifies harmonic functions, and transposes sequences using `parse_progression_string` and `transpose_progression`. Tools available: `your_tool_name`.

**Q: How do I use the transposition feature?**
Use `transpose_progression` by providing your original progression, the source key, and the target key.

**Q: Does it support chord extensions?**
Yes, you can use `get_chord_metadata` to retrieve detailed information including extensions like 7, 9, or 11.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roman-numeral-converter](https://vinkius.com/mcp/roman-numeral-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roman Numeral Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `roman-numeral-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roman Numeral Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roman-numeral-converter": {
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
