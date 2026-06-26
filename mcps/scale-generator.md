# Scale Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scale-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [music](../categories/music.md)

Generate detailed musical scale reports including intervals, enharmonics, and octave data.

## Description
The Scale Generator MCP connects AI agents to a powerful music theory engine. Use `generate_scale_report` to get structural breakdowns of scales across multiple octaves, including Roman numeral degrees and enharmonic equivalents. You can also use `list_available_scales` to discover over 4 much-needed scale families like Modes, Pentatonic, and Exotic, or `validate_musical_input` to check if a specific tonic and scale type are supported by the engine.


## Available Tools (3)
- **generate_scale_report**: g., "C") and a scale type from the catalog.

Generates a complete structural breakdown of a specific scale across multiple octaves
- **list_available_scales**: Allows discovery of the supported scales
- **validate_musical_input**: Validates whether a user's provided tonic and scale type are musically valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scale Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a report for C Major scale with 2 octaves."

**🤖 AI Agent:**
> The C Major scale (2 octaves) includes: I: C, II: D, III: E, IV: F, V: G, VI: A, VII: B. The second octave follows the same pattern starting from the next C.

---

**👤 You:**
> "What scales are available in the Pentatonic category?"

**🤖 AI Agent:**
> The available pentatonic scales include Major Pentatonic and Minor Pentatonic.

---

**👤 You:**
> "Is F# a valid tonic for the Lydian scale?"

**🤖 AI Agent:**
> Yes, F# is a valid tonic and the Lydian scale type is supported by the engine.


## ❓ FAQ

**Q: How can I see all supported scales?**
Use the `list_available_scales` tool to retrieve a categorized list of all available scale families and their members.

**Q: Can I generate scales for multiple octaves?**
Yes, when using `generate_scale_report`, you can provide an `octaveCount` parameter to specify how many octaves you want the report to cover.

**Q: Does it provide enharmonic equivalents?**
Yes, the `generate_scale_report` tool includes a list of enharmonic equivalents for every note in the scale to ensure musical accuracy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scale-generator](https://vinkius.com/mcp/scale-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scale Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scale-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scale Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scale-generator": {
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
