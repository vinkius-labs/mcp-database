# Mode Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mode-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Derive and explore the seven musical modes from any major or minor parent scale.

## Description
The Mode Calculator is a specialized tool for musicians and theorists to instantly generate the complete set of seven musical modes (Iontian, Dorian, Phrygian, Lydian, Mixolydian, Aeolian, and Locrian) from a provided parent scale. By using `generate_mode_set`, you can see every mode's notes, sonic texture, and typical genre. You can also use `analyze_mode_texture` to dive deep into the emotional character of a specific mode or `list_mode_notes` to extract just the note sequences. This tool bridges the gap between complex music theory and practical application in any AI-driven musical workflow.


## Available Tools (3)
- **list_mode_notes**: Provides the sequence of individual notes that make up a specific mode
- **generate_mode_set**: Generates the set of all 7 modes for a given parent scale
- **analyze_mode_texture**: g., Bright, Dark) and genre associated with a specific mode name.

Retrieves the sonic character and typical musical genre for a single specified mode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mode Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the modes for C Major."

**🤖 AI Agent:**
> For C Major, the modes are: Ionian (C D E F G A B), Dorian (D E F G A B C), Phrygian (E F G A B C D), Lydian (F G A B C D E), Mixolydian (G A B C D E F), Aeolian (A B C D E F G), and Locrian (B C D E F G A).

---

**👤 You:**
> "What is the texture of the Lydian mode in A Minor?"

**🤖 AI Agent:**
> The Lydian mode derived from A Minor has a bright sonic texture and is typically used in cinematic or dreamlike compositions.

---

**👤 You:**
> "List the notes for the Dorian mode in G Major."

**🤖 AI Agent:**
> The notes for the Dorian mode in G Major are: A, B, C, D, E, F#, G.


## ❓ FAQ

**Q: How do I generate all seven modes at once?**
Use the `generate_mode_set` tool by providing the name of your parent scale and selecting whether it is 'Major' or 'Minor'.

**Q: Can I see just the notes for a specific mode?**
Yes, use the `list_mode_notes` tool and specify the target mode name and its parent scale.

**Q: What information does the texture analysis provide?**
The `analyze_mode_texture` tool returns the sonic character (like bright or dark) and the typical musical genre associated with that mode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mode-calculator](https://vinkius.com/mcp/mode-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mode Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mode-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mode Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mode-calculator": {
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
