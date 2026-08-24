# Sudoku Grid Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sudoku-grid-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic engine for validating 9x9 Sudoku grid states and identifying rule violations.

## Description
This MCP server provides a deterministic engine to validate 9x9 Sudoku grids. It can check if a partial grid state is valid by identifying duplicate numbers in rows, columns, or 3x3 boxes, or determine if a fully filled grid is a solved puzzle. Use `validate_grid_state` to find specific rule violations like duplicate numbers, `check_completeness` to see if any cells are still empty, or `get_box_coordinates` to retrieve the cell indices for a specific 3x3 sub-grid.


## Available Tools (3)
- **check_completeness**: Quickly determines if the puzzle is ready to be evaluated as a finished solution
- **get_box_coordinates**: Maps a box index to its constituent cell coordinates for localized validation
- **validate_grid_state**: Checks if the current grid state adheres to Sudoku rules and identifies specific conflicts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sudoku Grid Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this Sudoku grid valid: [[5,3,0,0,7,0,0,0,0],[6,0,0,1,9,5,0,0,0],[0,9,8,0,0,0,0,6,0],[8,0,0,0,6,0,0,0,3],[4,0,0,8,0,3,0,0,1],[7,0,0,0,2,0,0,0,6],[0,6,0,0,0,0,2,8,0],[0,0,0,4,1,9,0,0,5],[0,0,0,0,8,0,0,7,9]]?"

**🤖 AI Agent:**
> The current grid state is valid, but it is not solved because there are empty cells.

---

**👤 You:**
> "Check if this grid has any duplicates: [[5,5,0,0,7,0,0,0,0],[6,0,0,1,9,5,0,0,0],[0,9,8,0,0,0,0,6,0],[8,0,0,0,6,0,0,0,3],[4,0,0,8,0,3,0,0,1],[7,0,0,0,2,0,0,0,6],[0,6,0,0,0,0,2,8,0],[0,0,0,4,1,9,0,0,5],[0,0,0,0,8,0,0,7,9]]"

**🤖 AI Agent:**
> The grid is invalid. Row 0 has duplicate 5.

---

**👤 You:**
> "How many empty cells are in this grid: [[1,2,3,4,5,6,7,8,9],[4,5,6,7,8,9,1,2,3],[7,8,9,1,2,3,4,5,6],[2,3,1,5,6,4,8,9,7],[5,6,4,8,9,7,2,3,1],[8,9,7,2,3,1,5,6,4],[3,1,2,6,4,5,9,7,8],[6,4,5,9,7,8,3,1,2],[9,7,8,3,1,2,6,4,5]]?"

**🤖 AI Agent:**
> The grid is fully filled with 0 empty cells.


## ❓ FAQ

**Q: How do I check if my Sudoku grid is valid?**
You can use the `validate_grid_state` tool by providing the 9x9 grid as a JSON string. It will return whether the state is valid and list any specific violations found.

**Q: Can this tool tell me if a Sudoku is fully solved?**
Yes, the `validate_grid_state` tool returns an `isSolved` boolean which is true only if the grid is valid and contains no empty cells (zeros).

**Q: How can I find the coordinates for a specific 3x3 box?**
Use the `get_box_coordinates` tool and provide the box index from 0 to 8 to get the row and column indices for that sub-grid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sudoku-grid-validator](https://vinkius.com/ai-agent-connect/sudoku-grid-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sudoku Grid Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sudoku-grid-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sudoku Grid Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sudoku-grid-validator": {
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
