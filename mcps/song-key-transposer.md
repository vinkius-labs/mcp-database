# Song Key Transposer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/song-key-transposer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transposes chord sequences between musical keys with accidental preference.

## Description
This MCP server provides tools to manipulate musical notation. Use `transpose_chords` to shift a sequence of chords from a source key to a target key, or `get_transposition_interval` to find the semitone distance between keys. It also includes `parse_chord_symbol` for breaking down chord components and `validate_key_existence` to ensure musical keys are valid.


## Available Tools (4)
- **validate_key_existence**: g., "C Major").

Verifies if a provided key name is a valid musical key
- **get_transposition_interval**: Determines the semitone distance between two keys
- **parse_chord_symbol**: g., "Bbmaj7").

Breaks down a single chord string into its constituent musical parts
- **transpose_chords**: Transposes a sequence of musical chords from one key to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Song Key Transposer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transpose the chords C, Am, F, G from C Major to G Major."

**🤖 AI Agent:**
> G, Em, C, D

---

**👤 You:**
> "What is the interval between Eb Minor and Bb Minor?"

**🤖 AI Agent:**
> 5

---

**👤 You:**
> "Break down the chord Bbmaj7."

**🤖 AI Agent:**
> Root: Bb, Accidental: b, Quality: maj7


## ❓ FAQ

**Q: How do I transpose a song?**
You can use the `transpose_chords` tool by providing the original chord sequence, the source key, and the target key.

**Q: Can I choose between sharps and flats?**
Yes, when using `transpose_chords`, you can set the `preferSharps` parameter to true or false to control the accidental preference.

**Q: What happens if I provide an invalid key?**
The `validate_key_existence` tool will check if the key is valid. If you attempt to transpose using an invalid key, the tool will return an error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/song-key-transposer](https://vinkius.com/en/ai-agent-connect/song-key-transposer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Song Key Transposer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `song-key-transposer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Song Key Transposer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "song-key-transposer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
