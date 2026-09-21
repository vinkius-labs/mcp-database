# Playlist BPM & Flow Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/playlist-bpm-flow-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Sequences songs by BPM, key, and energy to create smooth playlist transitions.

## Description
This MCP server provides a deterministic sequencing engine for music playlists. It uses musical attributes like BPM, key, and energy levels to calculate optimal song orders. Use `calculate_optimal_flow` to generate sequences based on policies like smooth ascent or energy waves. You can also use `analyze_transition_compatibility` to check if two specific songs fit together, or `validate_playlist_constraints` to ensure a sequence stays within specific energy and tempo limits.


## Available Tools (4)
- **analyze_transition_compatibility**: Evaluates how well two specific songs fit together
- **calculate_optimal_flow**: Generates a sequenced playlist based on a specific ordering strategy
- **get_alternative_sequence**: Provides a secondary ordering of the same songs using a different logic
- **validate_playlist_constraints**: Checks if a given sequence of songs violates specific hard constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Playlist BPM & Flow Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a smooth ascent playlist from these songs: [{'id': '1', 'bpm': 120, 'key': 'C', 'energy': 0.5, 'durationSeconds': 180}, {'id': '2', 'bpm': 124, 'key': 'G', 'energy': 0.6, 'durationSeconds': 200}]"

**🤖 AI Agent:**
> The optimal sequence is song 1 followed by song 2, with a total runtime of 380 seconds and a high compatibility score.

---

**👤 You:**
> "Are these two songs compatible: Song A (128 BPM, Am, 0.8 energy) and Song B (128 BPM, C, 0.7 energy)?"

**🤖 AI Agent:**
> Yes, the transition is smooth because the BPM is identical and the keys are harmonically related.

---

**👤 You:**
> "Check if this sequence of song IDs [101, 102, 103] violates a max energy delta of 0.2."

**🤖 AI Agent:**
> The sequence is valid and does not violate the energy delta constraint.


## ❓ FAQ

**Q: How do I create a smooth playlist?**
You can use the `calculate_optimal_flow` tool with a policy like 'smooth_ascent' to order your songs for a gradual increase in energy.

**Q: Can I check if two songs will sound good together?**
Yes, use `analyze_transition_compatibility` to evaluate the BPM, key, and energy relationship between two songs.

**Q: How can I prevent sudden jumps in my playlist?**
Use `validate_playlist_constraints` to check if your sequence violates maximum allowed deltas for BPM or energy levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/playlist-bpm-flow-calculator](https://vinkius.com/en/ai-agent-connect/playlist-bpm-flow-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Playlist BPM & Flow Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `playlist-bpm-flow-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Playlist BPM & Flow Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "playlist-bpm-flow-calculator": {
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
