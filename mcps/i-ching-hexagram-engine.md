# I Ching Hexagram Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/i-ching-hexagram-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate primary, transformed, and nuclear hexagrams from line values or coin tosses.

## Description
This MCP server provides a deterministic engine for the I Ching (Book of Changes). It allows AI agents to perform complex hexagram calculations, including identifying primary, transformed, and nuclear hexagrams. Users can provide direct line values (6, 7, 8, or 9) using `calculate_hexagram` or convert coin toss sequences into line values using `interpret_coin_toss`. The engine also supports retrieving specific trigram compositions via `get_trigram_details`.


## Available Tools (3)
- **calculate_hexagram**: Computes the full suite of hexagram data based on provided line values
- **get_trigram_details**: Retrieves the name and composition of a specific trigram
- **interpret_coin_toss**: g., "HHT") into the corresponding I Ching line values.

Converts a sequence of coin toss results into numeric line values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **I Ching Hexagram Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the hexagram for these line values: [7, 8, 7, 7, 8, 7]"

**🤖 AI Agent:**
> The primary hexagram is 11. Tai / Peace.

---

**👤 You:**
> "What is the hexagram for the coin toss sequence: ['HHT', 'TTH', 'HHH', 'TTT', 'HHT', 'TTH']?"

**🤖 AI Agent:**
> The resulting hexagram is 1. Qián / The Creative.

---

**👤 You:**
> "Tell me about the trigram 'Heaven'."

**🤖 AI Agent:**
> The trigram is Heaven, characterized by a pattern of three Yang lines.


## ❓ FAQ

**Q: What are the valid line values?**
The valid line values are 6 (Old Yin), 7 (Young Yang), 8 (Young Yin), and 9 (Old Yang).

**Q: How do I use coin tosses?**
You can use the `interpret_coin_toss` tool by providing an array of six 3-character strings representing the results of three coin tosses for each line.

**Q: What is a nuclear hexagram?**
A nuclear hexagram is a hidden hexagram derived from the internal lines (2-3-4 and 3-4-5) of the primary hexagram.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/i-ching-hexagram-engine](https://vinkius.com/ai-agent-connect/i-ching-hexagram-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **I Ching Hexagram Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `i-ching-hexagram-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **I Ching Hexagram Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "i-ching-hexagram-engine": {
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
