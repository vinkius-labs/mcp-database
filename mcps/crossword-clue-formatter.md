# Crossword Clue Formatter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crossword-clue-formatter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate deterministic metadata, symmetry checks, and statistics for crossword grids.

## Description
This MCP server provides precise tools for processing crossword puzzle grids. It allows AI agents to validate if a grid layout follows 180-degree rotational symmetry using `validate_grid_symmetry`, map clues to specific grid positions with `generate_clue_metadata`, and calculate structural properties like white square counts with `get_grid_statistics`. It is designed to ensure crossword data is consistent and correctly formatted.


## Available Tools (3)
- **get_grid_statistics**: Calculates the total letter capacity and structural properties of the grid
- **generate_clue_metadata**: Maps provided clues to their specific numbered positions and lengths within the grid
- **validate_grid_symmetry**: Checks if the provided grid layout follows the standard 180-degree rotational symmetry rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crossword Clue Formatter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the symmetry of this grid: [['#', 'A'], ['A', '#']]"

**🤖 AI Agent:**
> The grid layout follows 180-degree rotational symmetry.

---

**👤 You:**
> "What are the statistics for a 3x3 grid with one black square at the center?"

**🤖 AI Agent:**
> The grid has 8 white squares and dimensions of 3 rows by 3 columns.

---

**👤 You:**
> "Generate metadata for a grid with clues ['CAT', 'DOG']"

**🤖 AI Agent:**
> 1-Across (3 letters): CAT, 2-Down (3 letters): DOG.


## ❓ FAQ

**Q: How do I check if my crossword grid is symmetric?**
You can use the `validate_grid_symmetry` tool by providing your grid as a 2D array of strings.

**Q: Can I get the total number of white squares in my grid?**
Yes, the `get_grid_statistics` tool calculates the total white square count and grid dimensions.

**Q: How are clues numbered?**
The `generate_clue_metadata` tool assigns numbers sequentially starting from 1, following standard crossword rules for Across and Down words.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crossword-clue-formatter](https://vinkius.com/ai-agent-connect/crossword-clue-formatter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crossword Clue Formatter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crossword-clue-formatter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crossword Clue Formatter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crossword-clue-formatter": {
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
