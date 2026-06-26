# Circle of Fifths Navigator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circle-of-fifths-navigator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Navigate musical keys, identify tonal relationships, and plan modulations using the Circle of Fifverts framework.

## Description
The Circle of Fifths Navigator is a specialized tool for musicians to explore musical keys and their relationships. Using tools like `get_key_neighbors`, you can instantly find the dominant and subdominant keys, as well as relative major and minor scales. The `get_key_signature_details` tool provides technical details including accidental order and available modes. For more complex compositions, use `calculate_modulation_paths` to identify natural modulation paths based on distance on the circle, or `get_enharmonic_mapping` to find equivalent keys with different notation.


## Available Tools (4)
- **get_enharmonic_mapping**: Answers "Is there a different way to write this key using different notation?"
- **get_key_neighbors**: g., "G Major", "Eb Minor") and returns its dominant, subdominant, relative major, and relative minor.

Answers "Who are the closest musical relatives and neighbors to this specific key?"
- **get_key_signature_details**: Answers "What are the technical components of this key's scale and its available modes?"
- **calculate_modulation_paths**: Answers "Which keys can I move to for a natural modulation, and how far away are they?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circle of Fifths Navigator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are the closest musical relatives and neighbors to G Major?"

**🤖 AI Agent:**
> For G Major, the dominant key is D Major, the subdominant is C Major, the relative minor is E Minor, and the relative major is G Major.

---

**👤 You:**
> "What are the technical components of Eb Minor?"

**🤖 AI Agent:**
> Eb Minor has 6 flats (Bb, Eb, Ab, Db, Gb, Cb) and includes modes such as Aeolian, Dorian, and Phrygian.

---

**👤 You:**
> "Find a natural modulation path from C Major with a max distance of 1."

**🤖 AI Agent:**
> From C Major, you can naturally modulate to G Major (distance +1) and F Major (distance -1).


## ❓ FAQ

**Q: How can I find the closest musical relatives to a specific key?**
Use the `get_key_neighbors` tool by providing the name of your starting key (e.g., 'G Major'). It will return the dominant, subdominant, and relative major/minor keys.

**Q: How do I identify natural modulation paths for a song?**
Use the `calculate_modulation_paths` tool. By specifying a starting key and a maximum distance, you can see which keys are reachable with 'Immediate' or 'Adjacent' difficulty levels.

**Q: Can this tool help me understand key signatures?**
Yes, the `get_key_signature_details` tool provides the exact order of sharps or flats, the total count of accidentals, and the available modes for any given key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circle-of-fifths-navigator](https://vinkius.com/mcp/circle-of-fifths-navigator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circle of Fifths Navigator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circle-of-fifths-navigator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circle of Fifths Navigator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circle-of-fifths-navigator": {
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
