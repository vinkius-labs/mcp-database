# Relative & Parallel Key Finder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/relative-parallel-key-finder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Instantly discover relative, parallel, and related musical keys based on any input key.

## Description
The Relative & Parallel Key Finder is a powerful music theory utility that connects AI agents to the structural relationships of Western music. By using tools like `find_key_relationships`, you can instantly identify relative and parallel keys, homonymous keys, and keys at a third-distance interval. You can also use `get_signature_details` to inspect the technical composition of any key's signature (sharps, flats, or none) and `lookup_modulation_guide` to access a complete reference table for modulation planning. This MCP server acts as a bridge between your AI assistant and complex music theory logic, making it perfect for composers, students, and musicians working in Cursor, VS Code, Claude Desktop, or Windsurf.


## Available Tools (3)
- **find_key_relationships**: Returns relative, parallel, antiparallel, homonymous, and third-distance keys.

Provides a complete set of relations for a given key
- **get_signature_details**: Returns accidental count, type (sharps/flats/none), and mode.

Describes the technical composition of a key's signature
- **lookup_modulation_guide**: Provides a comprehensive reference table of all key signatures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative & Parallel Key Finder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the relative and parallel key of G Major?"

**🤖 AI Agent:**
> The relative key of G Major is E Minor, and its parallel key is G Minor.

---

**👤 You:**
> "How many sharps are in the key of D Major?"

**🤖 AI Agent:**
> D Major has 2 sharps (F# and C#).

---

**👤 You:**
> "Show me all keys that share the same tonic as Eb Major."

**🤖 AI Agent:**
> The homonymous keys for Eb Major are Eb Major and Eb Minor.


## ❓ FAQ

**Q: How can I find the relative key of C Major?**
You can use the `find_key_relationships` tool with 'C Major' as the input. It will return A Minor as the relative key.

**Q: What does `get_signature_details` provide?**
It provides the number of accidentals, whether they are sharps or flats, and identifies if the key is Major or Minor.

**Q: Can I use this for modulation planning?**
Yes, the `lookup_modulation_guide` tool provides a complete reference table of all key signatures to assist in finding suitable keys for modulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/relative-parallel-key-finder](https://vinkius.com/mcp/relative-parallel-key-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative & Parallel Key Finder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-parallel-key-finder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative & Parallel Key Finder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-parallel-key-finder": {
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
