# Transposition Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transposition-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transpose notes, chords, scales, and progressions with ease.

## Description
A specialized musical engine for precise transposition. Use `transpose_element` to shift individual notes or chords, `apply_instrument_notation` to adapt concert pitch for Bb, Eb, and F instruments, `resolve_enharmonic_spelling` to ensure correct notation in specific keys, and `transpose_progression` to move entire sequences of music at once.


## Available Tools (4)
- **transpose_element**: Transpose a single musical element
- **apply_instrument_notation**: Apply notation for transposing instruments
- **resolve_enharmonic_spelling**: Resolve enharmonic spelling
- **transpose_progression**: Transpose a musical progression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transposition Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transpose the note C to 2 semitones up."

**🤖 AI Agent:**
> D

---

**👤 You:**
> "What is the written notation for a concert pitch of Eb for an Alto Saxophone?"

**🤖 AI Agent:**
> C

---

**👤 You:**
> "Transpose this progression: ['C', 'Am', 'F', 'G'] by -2 semitones."

**🤖 AI Agent:**
> ['Bb', 'Gm', 'Eb', 'F']


## ❓ FAQ

**Q: What musical elements can I transpose?**
You can transpose individual notes, chords (including complex qualities like maj7), scales, and entire progressions using the `transpose_element` or `transpose_progression` tools.

**Q: How does it handle transposing instruments?**
The `apply_instrument_notation` tool automatically calculates the correct written notation for Bb (e.g., Trumpet), Eb (e.g., Alto Sax), and F (e.g., French Horn) instruments based on a provided concert pitch.

**Q: Can it resolve enharmonic duplicates?**
Yes. By using `resolve_enharmonic_spelling`, you can provide a scale context (like 'G Major') to ensure that notes like A# are correctly spelled as Bb for better musical readability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transposition-calculator](https://vinkius.com/mcp/transposition-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transposition Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transposition-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transposition Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transposition-calculator": {
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
